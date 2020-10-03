# Experiment 2: Jenkins integration with GitHub

## Steps Performed

- Start Jenkins. Goto -> [localhost](https://localhost:8080).

![Screenshot from 2020-08-28 09-28-55](https://user-images.githubusercontent.com/46739435/95686817-05282000-0c1e-11eb-9823-90f4b3931903.png)
![Screenshot from 2020-08-28 09-30-18](https://user-images.githubusercontent.com/46739435/95686818-05c0b680-0c1e-11eb-9eb5-7876bc93c841.png)

- Create new jenkins job.

- Mark git in Source Code Management and add URL of Repo.
![Screenshot from 2020-08-28 09-32-18](https://user-images.githubusercontent.com/46739435/95686820-078a7a00-0c1e-11eb-8776-c268ec120818.png)

- Poll SCM to trigger automatically on commit.
![Screenshot from 2020-08-28 10-35-01](https://user-images.githubusercontent.com/46739435/95687205-de6ae900-0c1f-11eb-9625-6a5ff801541c.png)

- Make changes to git repo and push it GitHub.
![Screenshot from 2020-08-28 09-36-27](https://user-images.githubusercontent.com/46739435/95686826-0bb69780-0c1e-11eb-9aaf-0fc0eba352d6.png)

- Check build status in Jenkins. Your projeect will be cloned in jenkins home directory.
![Screenshot from 2020-08-28 10-26-23](https://user-images.githubusercontent.com/46739435/95686829-0d805b00-0c1e-11eb-9962-a1bf0f4535b5.png)
