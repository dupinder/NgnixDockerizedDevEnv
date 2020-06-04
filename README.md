# Development environment with containers

This repository contains all the required files and configuration which help you to setup a containerized enviournment, which have a UI application in different container and a backend application in different container. Both the applications are communication using Ngnix server. 

Ngnix reverse-proxy configuration is described in detail.


**Setup Instructions:**

1. Update repositories backend and repos with latest code.
2. Clean build your backend and UI app.
3. Replace placeholder `[ ... ]` in docker-compose.yml file, as described in comments.
4. Open docker-compose.yml, in each and every step I added comments. and suggests changes.
5. Like we I go throght docker-compose in backend service, You just need to map app build path to the volumn and pass build Jar Name
6. In UI App, Just pass the UI build path. Exhibit in case of Angular App "E:\repos\ui-app\dist\ui-app"
    
* How to Run:

  Open powershell in the root dir of current Repo/localDevEnv and run following command

  ```
  docker-compose -f "docker-compose.yml" up -d --build

  command complete with output:

  Creating beservice ... done
  Creating uiapp     ... done 

  ```