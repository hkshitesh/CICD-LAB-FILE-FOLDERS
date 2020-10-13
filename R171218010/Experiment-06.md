# Experiment 6: Create a pipeline using JenkinsFile

## Steps Performed

- Create a simple maven project.

- Create a Jenkinsfile.
```
pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo 'Build Stage'
            }
        }
        stage('clean stage'){
            steps{
                sh 'cd jenkins_file && mvn clean'
            }
        }
        stage('package'){
            steps{
                sh 'cd jenkins_file && mvn package'
            }
        }
        stage('package upload'){
            steps{
                sh 'git add .'
                sh 'git commit -m "Commit from jenkins"'
                sh 'git push origin jenkins_file'
            }
        }
    }
}
```
![Screenshot from 2020-08-28 12-39-18](https://user-images.githubusercontent.com/46739435/95735565-980a9e00-0ca2-11eb-884e-f25686408b50.png)

- Commit changes and push to GitHub.

- Goto [Jenkins](http://localhost:8080/)

- Click on create new item.

- Enter an item name and select Pipeline.

- Select git in SCM and Enter repo URL.
![Screenshot from 2020-08-28 12-38-20](https://user-images.githubusercontent.com/46739435/95735558-96d97100-0ca2-11eb-8c2c-46d31819b18f.png)

- Poll SCM to trigger automated builds.

- Enter Jenkinsfile path in script path.
![Screenshot from 2020-08-28 12-38-20](https://user-images.githubusercontent.com/46739435/95735558-96d97100-0ca2-11eb-8c2c-46d31819b18f.png)

- Check builds.
![Screenshot from 2020-08-28 12-38-08](https://user-images.githubusercontent.com/46739435/95735553-950fad80-0ca2-11eb-8080-b6c1b9d4a46e.png)

- Check console output.
![Screenshot from 2020-08-28 12-46-55](https://user-images.githubusercontent.com/46739435/95735576-99d46180-0ca2-11eb-87c6-6ea97e4d9565.png)
