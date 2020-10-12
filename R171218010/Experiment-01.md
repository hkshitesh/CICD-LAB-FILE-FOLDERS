# Experiment 1: Installation of Jenkins and Execution of simple job in Jenkins

## Steps Performed

### Installing Jenkins
 - Install Jenkins using `sudo apt install jenkins`
![Screenshot from 2020-10-04 02-31-11](https://user-images.githubusercontent.com/46739435/95001692-ffad5300-05e9-11eb-9845-0a1293ed5efb.png)


- Start Jenkins using command `sudo systemctl start jenkins`and enable service using `sudo systemctl enable jenkins`![Screenshot from 2020-10-04 02-37-30](https://user-images.githubusercontent.com/46739435/95001756-a42f9500-05ea-11eb-8375-01470baf10bd.png)

- Access jenkins from your browser at [https://localhost:8080](https://localhost:8080).
- Create user if fresh install otherwise login.
![Screenshot from 2020-10-04 02-39-19](https://user-images.githubusercontent.com/46739435/95002033-6e3fe000-05ed-11eb-8d37-79a6bdbe8e89.png)
- Jenkins Homepage
![Screenshot from 2020-10-04 02-53-33](https://user-images.githubusercontent.com/46739435/95001963-d0e4ac00-05ec-11eb-8eca-a255002261e2.png)

### Create a simple Job
- Create a new job.
- Opt for freestyle project.
![Screenshot from 2020-10-04 03-08-54](https://user-images.githubusercontent.com/46739435/95002199-fd012c80-05ee-11eb-8caf-edef5b17a58c.png)
- Execute shell command
![Screenshot from 2020-10-04 03-16-00](https://user-images.githubusercontent.com/46739435/95002302-faeb9d80-05ef-11eb-8724-7ad23455e891.png)
- Click save and apply
- Click on Build Now to initiate build.
![Screenshot from 2020-10-04 03-16-11](https://user-images.githubusercontent.com/46739435/95002324-253d5b00-05f0-11eb-807e-3c9e868303b5.png)
- Console Output
![Screenshot from 2020-10-04 03-16-33](https://user-images.githubusercontent.com/46739435/95002329-38502b00-05f0-11eb-912b-0282d32ba414.png)
