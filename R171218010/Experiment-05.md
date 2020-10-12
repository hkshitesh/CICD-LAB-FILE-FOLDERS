# Experiment 6: Jenkins Integration with SonarQube

## Steps Performed

- Goto [Jenkins](http://localhost:8080/)

- Click on create new item.

- Enter an item name and select Maven project.
![Screenshot from 2020-10-12 15-20-54](https://user-images.githubusercontent.com/46739435/95734401-0b131500-0ca1-11eb-8429-1d71bb638bcc.png)

- Select git in SCM and Enter repo URL.
![Screenshot from 2020-10-12 15-34-29](https://user-images.githubusercontent.com/46739435/95734415-0ea69c00-0ca1-11eb-86c1-73a8f93beab2.png)

- Setup build goal in maven column ``` clean install sonar:sonar -Dsonar.host.url=http://192.168.99.100:9000 -Dsonar.analysis.mode=publish ```
![Screenshot from 2020-10-12 15-34-37](https://user-images.githubusercontent.com/46739435/95734421-0fd7c900-0ca1-11eb-97cd-f16207a41ff5.png)

- Click on build now.
![Screenshot from 2020-10-12 15-36-57](https://user-images.githubusercontent.com/46739435/95734427-1108f600-0ca1-11eb-9cfa-da113bd33049.png)

- Check console output of previous build.
![Screenshot from 2020-10-12 15-37-52](https://user-images.githubusercontent.com/46739435/95734431-123a2300-0ca1-11eb-809d-4b1f65736d6b.png)

- Your maven project would be uploaded to SonarQube successfully.
![Screenshot from 2020-10-12 15-37-57](https://user-images.githubusercontent.com/46739435/95734436-136b5000-0ca1-11eb-9590-c3995748d4cc.png)
