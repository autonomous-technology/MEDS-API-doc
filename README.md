# MEDS-API-doc
## Add APIs to Swagger UI
1. Needs to run [Swagger UI](https://swagger.io/docs/open-source-tools/swagger-ui/usage/installation/) on your local machine. Preferably, setup from Docker:
    ```shell
    docker pull swaggerapi/swagger-ui
    docker run -p 80:8080 -e SWAGGER_JSON=/mount/swagger.json -v FULL_PATH:/mount swaggerapi/swagger-ui
    ```
   **IMPORTANT:** Change variable `FULL_PATH` with an absolute path for the folder where swagger.json locates.
2. Open http://localhost or 127.0.0.1 in your browser to use Swagger UI with MEDS APIs.

## Generate client-side code for APIs
1. Needs to run [Swagger Editor](https://swagger.io/docs/open-source-tools/swagger-editor/) on your local machine. Preferably, setup from Docker:
    ```shell
   docker pull swaggerapi/swagger-editor
   docker run -p 80:8080 swaggerapi/swagger-editor
    ```
2. After starting the docker container, open http://localhost or 127.0.0.1 in your browser to use Swagger Editor.
3. Import [swagger.json](swagger.json) file by selecting File -> Import file
4. On the right side of the screen, you will see Swagger UI with the MEDS APIs
5. You can generate client-side code for MEDS APIs. Select Generate Client and make your choice.
