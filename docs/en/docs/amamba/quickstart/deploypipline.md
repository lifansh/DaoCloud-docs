# Quickly create a pipeline

This section will create a pipeline by compiling, building, and deploying, and will help you quickly create a pipeline through detailed step-by-step descriptions.

## Prerequisites

- Need to create a workspace and a user, the user needs to join the workspace and give `workspace edit` role. Refer to [Creating Workspaces](../../ghippo/user-guide/workspace/Workspaces.md), [Users and Roles](../../ghippo/user-guide/access-control/User.md).
- Create two credentials that can access the container registry and the cluster, named respectively: `registry`, `kubeconfig`. For more information on creating credentials, please refer to [Credential Management](../user-guide/Pipeline/Credential.md).
- Prepare a GitHub repository, DockerHub repository.

## Create Credentials

1. Create two credentials on the Credentials page:

    - docker-credential: username and password for accessing the container registry.
    - demo-dev-kubeconfig: used to access the Kubernetes cluster using this kubeconfig.

2. After the creation is complete, you can see the credential information on the `Certificate List` page.

## Create a custom pipeline

1. Click `Create Pipeline` on the pipeline list page.

    

2. In the pop-up dialog box, select Custom Create Pipeline and click OK.

    

3. Enter the `custom pipeline creation page`, and enter the pipeline name `pipeline-demo`.

    

4. Add three string parameters in `Build Parameters`, these parameters will be used in the image build command.

    - registry: container registry address. Example value: `release.daocloud.io`.
    - project: The name of the project in the container registry. Example value: `demo`.
    - name: The name of the image. Example value: `http-hello`.

    

5. After adding, click `OK`.

## Edit pipeline

1. Click the name of a pipeline on the pipeline list page.

    

2. Click `Edit Pipeline` in the upper right corner,

    

3. Click `Global Settings` in the upper right corner.

    

4. Set the type to node and the label to go, click `OK`.

    

5. Add stage - pull source code.

    - Click on `Add Stage` in the canvas. In the stage settings on the right set the name: git clone.
    - Click `Add Step`, select git clone under the step type in the pop-up dialog box, and configure related parameters:
        - Repository URL: Enter the GitLab repository address.
        - Branch: if not filled in, the default is the master branch.
        - Credentials: If it belongs to a private registry, you need to provide a credential.

    

6. Add stage - build and push the image.

    - Click on `Add Stage` in the canvas. Set the name in the stage settings on the right: build & push.

    - In the step module, select to enable `specify container`, fill in the container name: go in the pop-up dialog box, and then click `OK`.

        

    - Select to enable `Use Credentials` in the step module, fill in the relevant parameters in the pop-up dialog box, and then click `OK`.

        - Credentials: Select the created Docker hub credentials to allow users to access the container registry.
        - Password variable: PASS
        - Username variable: USER

        

    - Click `Add Step` to build the code, select shell under the step type in the pop-up dialog box, enter the following command in the command line, and then click `OK`.

        ```go
        go build -o simple-http-server main.go
        ```

    - Click `Add Step` to build the Docker image according to the Dockerfile in the source code, select shell under the step type in the pop-up dialog box, enter the following command in the command line, and click `OK`.

        ```docker
        docker build -f Dockerfile . -t $registry/$project/$name:latest
        ```

    - Click `Add Step` to log in to the container registry, select shell under the step type in the pop-up dialog box, enter the following command in the command line, and then click `OK`.

        ```docker
        docker login $registry -u $USER -p $PASS
        ```

    - Click `Add Step` to push the image to the container registry, select shell under the step type in the pop-up dialog box, enter the following command in the command line, and click `OK`.

        ```docker
        docker push $registry/$project/$name:latest
        ```

7. Add stage - deploy to cluster

    - Click on `Add Stage` in the canvas. In the stage settings on the right set the name: deploy.

    - In the step module, select to enable `specify container`, fill in the container name: go in the pop-up dialog box, and then click `OK`.

        

    - Select to enable `Use Credentials` in the step module, fill in the relevant parameters in the pop-up dialog box, and then click `OK`.

         - Credentials: Choose a credential of type kubeconfig.

         - kubeconfig variable: If you are using the kubectl apply deployment method, the variable value must be KUBECONFIG.

         

    - Click `Add Step` to perform the cluster deployment operation, select shell under the step type in the pop-up dialog box, enter the following command in the command line, and click `OK`.

        ```shell
        kubectl apply -f deploy.yaml
        ```

## Save and execute the pipeline pipeline

1. Click `Save and Execute` after completing the previous step.

    

2. In the displayed dialog box, enter the sample parameters in step 2. Click `OK` to run the pipeline successfully.

    