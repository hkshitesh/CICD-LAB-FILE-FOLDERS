# Experiment 10: Uploading Artifacts on Nexus Server using CLI

## Steps Performed

- [Install Nexus](https://help.sonatype.com/repomanager3/installation/run-as-a-service)

- Nexus will be accessible to localhost at port 8081 *by default*. [Open Nexus](http://localhost:8081/)
  ![Screenshot from 2020-10-13 01-42-55](https://user-images.githubusercontent.com/46739435/95786553-725ab480-0cf5-11eb-8bf7-76e5f941a7f8.png)

- Goto: Server administration and configuration -> Repositories tab
  ![Screenshot from 2020-10-13 01-45-18](https://user-images.githubusercontent.com/46739435/95786717-c49bd580-0cf5-11eb-8e57-1775a1b18fb0.png)

- Click on create repository.

- Select maven2 (hosted)
  ![Screenshot from 2020-10-13 01-46-57](https://user-images.githubusercontent.com/46739435/95786850-0167cc80-0cf6-11eb-9543-fdae1049b628.png)

- Configure repository by adding required details.
  ![Screenshot from 2020-09-26 09-35-32](https://user-images.githubusercontent.com/46739435/95786985-3d029680-0cf6-11eb-978b-40a0124f0910.png)
  
- Add nexus credentials to ```~/m2/settings.xml```.
  ```
  <servers>
    <!-- .... -->
          <server>
                <id>CICD</id>
                <username>admin</username>
                <password>redhat</password>
        </server>
   </servers>

  ```
  
- Add configuration to pom.xml in maven project.
  ```
  <project>
    <!-- .... -->
      <distributionManagement>
        <snapshotRepository>
          <id>CICD</id>
          <name>CICD</name>
          <url>http://localhost:8081/repository/CICD/</url>
        </snapshotRepository>
      </distributionManagement>
  </project>
  ```
  
- Run ``` mvn deploy ``` from maven project.
  ![Screenshot from 2020-09-26 09-41-16](https://user-images.githubusercontent.com/46739435/95787554-6112a780-0cf7-11eb-932e-4dbf8cc783ab.png)
  ![Screenshot from 2020-09-26 09-55-25](https://user-images.githubusercontent.com/46739435/95787560-653ec500-0cf7-11eb-9f8c-38722e619cca.png)

- Your build will created an deployed at nexus server.
  ![Screenshot from 2020-09-26 09-57-24](https://user-images.githubusercontent.com/46739435/95787630-8b646500-0cf7-11eb-9341-37c59b77d2d6.png)
  ![Screenshot from 2020-09-26 09-57-35](https://user-images.githubusercontent.com/46739435/95787632-8dc6bf00-0cf7-11eb-8e8a-f88c11959dea.png)

