# Experiment 14: Dockerfile, Docker image and Docker Hub

## Steps Performed

- Create a directory to perform experiment using ```mkdir dirpath``` and ```cd``` to switch to that directory.
![Screenshot from 2020-12-03 12-39-19](https://user-images.githubusercontent.com/46739435/101075293-d435ed00-35c7-11eb-898f-20e0a6a0d62b.png)

- Create and open a file with name Dockerfile. Using ```vim Dockerfile```

- Add instructions for Dockerfile.                  
![Screenshot from 2020-12-03 12-32-25](https://user-images.githubusercontent.com/46739435/101075514-2119c380-35c8-11eb-9930-73d721753e31.png)

- Build docker image using ```sudo docker build -t nginx-server:v1 .```
![Screenshot from 2020-12-03 12-49-52](https://user-images.githubusercontent.com/46739435/101077208-8a023b00-35ca-11eb-8918-e56092f90e8b.png)

- Your image will build.                       
![Screenshot from 2020-12-03 12-50-22](https://user-images.githubusercontent.com/46739435/101077317-b027db00-35ca-11eb-8f8b-6d914c611d10.png)

- Build image can simply run using ```docker run``` command.
![Screenshot from 2020-12-03 18-52-15](https://user-images.githubusercontent.com/46739435/101077508-efeec280-35ca-11eb-835d-cbe1340c6a15.png)

- Test page from docker.                      
![Screenshot from 2020-12-03 18-52-31](https://user-images.githubusercontent.com/46739435/101077554-0006a200-35cb-11eb-8e26-904837b54f9b.png)

- Build docker image can be uploaded to docker hub by doing ```docker login``` and then using ```docker push``` command to upload the image.
![Screenshot from 2020-12-03 14-35-15](https://user-images.githubusercontent.com/46739435/101077880-71deeb80-35cb-11eb-94d3-9a09930132f2.png)
![Screenshot from 2020-12-03 14-35-31](https://user-images.githubusercontent.com/46739435/101077926-7e634400-35cb-11eb-8d3d-53dda4c5dd30.png)
