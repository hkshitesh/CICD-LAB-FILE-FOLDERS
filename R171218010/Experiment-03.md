# Experiment 3: Jenkins integration with GitHub and Maven

## Steps Performed

- Create a maven project.
![Screenshot from 2020-08-28 09-22-49](https://user-images.githubusercontent.com/46739435/95686811-fe011200-0c1d-11eb-9d31-6d99789a6224.png)
![Screenshot from 2020-08-28 09-26-49](https://user-images.githubusercontent.com/46739435/95686814-022d2f80-0c1e-11eb-82f5-5fc6a26882e9.png)

- Start Jenkins. Goto -> [localhost](https://localhost:8080).

![Screenshot from 2020-08-28 09-28-55](https://user-images.githubusercontent.com/46739435/95686817-05282000-0c1e-11eb-9823-90f4b3931903.png)
![Screenshot from 2020-08-28 09-30-18](https://user-images.githubusercontent.com/46739435/95686818-05c0b680-0c1e-11eb-9eb5-7876bc93c841.png)

- Create new maven pipeline.

- Mark git in Source Code Management and add URL of Repo.
![Screenshot from 2020-08-28 09-32-18](https://user-images.githubusercontent.com/46739435/95686820-078a7a00-0c1e-11eb-8776-c268ec120818.png)

- Configure Build settings.
![Screenshot from 2020-08-28 09-32-21](https://user-images.githubusercontent.com/46739435/95686823-09ecd400-0c1e-11eb-9262-6c68d27e0f9d.png)

- Poll SCM to trigger automatically on commit.
![Screenshot from 2020-08-28 10-35-01](https://user-images.githubusercontent.com/46739435/95687205-de6ae900-0c1f-11eb-9625-6a5ff801541c.png)

- Make changes to maven project and push it GitHub.
![Screenshot from 2020-08-28 09-36-27](https://user-images.githubusercontent.com/46739435/95686826-0bb69780-0c1e-11eb-9aaf-0fc0eba352d6.png)

- Check build status in Jenkins.
![Screenshot from 2020-08-28 10-26-23](https://user-images.githubusercontent.com/46739435/95686829-0d805b00-0c1e-11eb-9962-a1bf0f4535b5.png)
![Screenshot from 2020-08-28 10-26-38](https://user-images.githubusercontent.com/46739435/95687178-a95e9680-0c1f-11eb-9c78-c54f20af2252.png)
