# docker-spfx
Create a development environment for SharePoint Framework (SPFx) with a Docker container.  

1. **Clone this repository** to a directory of your choice.  
1. Move to the **docker-spfx** directory.  
1. Execute the following command to start the container.  

    ```bash
    docker-compose up -d --build
    ```

1. Run the following command to confirm that the container has started.  

    ```bash
    docker-compose ps
    ```

# Creating SPFx Solution
Create a SPFx solution using the docker-compose command.  

```bash
docker-compose run --rm app yo @microsoft/sharepoint
```
For more information on creating solution files, see [here](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview).  