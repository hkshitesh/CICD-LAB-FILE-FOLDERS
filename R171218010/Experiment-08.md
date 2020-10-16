# Experiment 8: Implement Master/Slave architecture in Jenkins

## Steps Performed

- Create a working directory for jenkins-slave-2 ```mkdir dir_name```

- Add Slave to Jenkins:  Manage Jenkins -> Manage Nodes and Clouds -> Click on New Node.

- Add **Node Name** and select **Permanent Agent**.
  ![Screenshot from 2020-10-13 01-15-26](https://user-images.githubusercontent.com/46739435/95784513-9a481900-0cf1-11eb-942d-7ee4e7226843.png)

- Add **Remote root directory** *(dir_path_created_step_1)*.

- Select **Launch method** *Launch agent by connecting it to master*.

- Add **Custom WorkDir path** *(dir_path_created_step_1)*.
  ![Screenshot from 2020-10-13 01-20-44](https://user-images.githubusercontent.com/46739435/95785061-ae404a80-0cf2-11eb-8b86-3b62f0fe4b51.png)

- Download [agent.jar](http://localhost:8080/jnlpJars/agent.jar)

- Run Command (given at slave dashboard): ``` java -jar agent.jar -jnlpUrl http://localhost:8080/computer/Slave%201/slave-agent.jnlp -secret 2*********************************5 -workDir "(dir_path_created_step_1)" ``` 
  ![Screenshot from 2020-09-11 11-34-16](https://user-images.githubusercontent.com/46739435/95784331-3b829f80-0cf1-11eb-9545-b5db4cc35e63.png)

- Create a new job.
  ![Screenshot from 2020-09-11 11-33-11](https://user-images.githubusercontent.com/46739435/95784328-39b8dc00-0cf1-11eb-9e96-31ab45e629af.png)

- Checkmark *Restrict where this project can be run* <br>
  **Label Expression:** Node Name
  ![Screenshot from 2020-09-11 11-33-02](https://user-images.githubusercontent.com/46739435/95784321-37ef1880-0cf1-11eb-97e1-4b3fd76e335e.png)
  
- Build Project.

- Check Projects tied to Slave1 from Manage Node. Your project would be listed there.
![Screenshot from 2020-09-11 11-34-27](https://user-images.githubusercontent.com/46739435/95784334-3c1b3600-0cf1-11eb-88e8-ff939d9cd7c9.png)
