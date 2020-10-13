# Experiment 4: Static Code analysis using SonarQube

## Steps Performed

- Download [SonarQube](https://www.sonarqube.org/)
![Screenshot from 2020-10-12 14-58-28](https://user-images.githubusercontent.com/46739435/95730380-ce90ea80-0c9b-11eb-980f-b68d45862429.png)

- Extract it
![Screenshot from 2020-10-12 14-45-30](https://user-images.githubusercontent.com/46739435/95730343-c33dbf00-0c9b-11eb-919e-4196456ba4d6.png)

- Execute StartSonar.bat to run SonarQube
![Screenshot from 2020-10-12 14-46-54](https://user-images.githubusercontent.com/46739435/95730355-c638af80-0c9b-11eb-818c-67841f7ed87c.png)

- SonarQube would be accessible at [localhost](https://localhost:9000) at port number 9000. Default **id:** *admin* **passwd:** *admin*
![Screenshot from 2020-10-12 14-52-47](https://user-images.githubusercontent.com/46739435/95730357-c6d14600-0c9b-11eb-933a-598ccc5ec23c.png)

- Use command ``` mvn clean install sonar:sonar -Dsonar.host.url=http://localhost:9000 -Dsonar.analysis.mode=publish ``` to deploy maven project to SonarQube
![Screenshot from 2020-10-12 14-55-18](https://user-images.githubusercontent.com/46739435/95730362-c89b0980-0c9b-11eb-9eec-d3f10c397c7b.png)
![Screenshot from 2020-10-12 14-55-32](https://user-images.githubusercontent.com/46739435/95730366-c9cc3680-0c9b-11eb-9eea-58f49f1bf15e.png)

- Deployed code can be seen on SonarQube pannel.
![Screenshot from 2020-10-12 14-55-57](https://user-images.githubusercontent.com/46739435/95730369-cb95fa00-0c9b-11eb-9996-6c5418005777.png)

- Click on the project to analyse code.
![Screenshot from 2020-10-12 14-56-19](https://user-images.githubusercontent.com/46739435/95730374-ccc72700-0c9b-11eb-9b67-c06fd3709530.png)
