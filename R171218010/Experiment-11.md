# Experiment 11: Vagrant

## Steps Performed

- Install VirtualBox. [Download](https://www.virtualbox.org/wiki/Downloads)
![Screenshot from 2020-11-27 02-55-50](https://user-images.githubusercontent.com/46739435/100392289-14dbb680-305c-11eb-8529-67f8ec3b7357.png)

- Install vagrant  ```sudo apt install vagrant```
![Screenshot from 2020-11-27 02-57-06](https://user-images.githubusercontent.com/46739435/100392358-4b193600-305c-11eb-93de-02341e9ecf3b.png)

- Run ```vagrant --version``` to verify install.
![Screenshot from 2020-11-27 02-58-38](https://user-images.githubusercontent.com/46739435/100392408-76038a00-305c-11eb-80e6-92b25271d280.png)

- Create a directory and change to that directory using ```mkdir & cd```
![Screenshot from 2020-11-27 02-59-53](https://user-images.githubusercontent.com/46739435/100392465-a3e8ce80-305c-11eb-847b-71e88051a3af.png)

- Initial vagrant using ```vargant init```
![Screenshot from 2020-11-27 03-01-05](https://user-images.githubusercontent.com/46739435/100392513-cda1f580-305c-11eb-9059-371d30af118c.png)

- Edit Vagrantfile created just now using ```vim Vagrantfile```
![Screenshot from 2020-11-27 03-04-07](https://user-images.githubusercontent.com/46739435/100392629-3a1cf480-305d-11eb-9f96-5eecef7be502.png)

- Set config.vm.box = "hashicorp/precise64"
![Screenshot from 2020-11-27 03-04-23](https://user-images.githubusercontent.com/46739435/100392648-45702000-305d-11eb-81dc-ce4510c5b00b.png)

- Run ```vagrant up``` to run vagrant and create vm.
![Screenshot from 2020-11-27 03-05-19](https://user-images.githubusercontent.com/46739435/100392739-89fbbb80-305d-11eb-887c-e3bdd2ae7370.png)

- Use ```vagrant ssh``` to get remote of create VM.

- Run ```vagrant halt``` to stop VM.
![Screenshot from 2020-11-27 03-14-22](https://user-images.githubusercontent.com/46739435/100393141-af3cf980-305e-11eb-96f7-f210ee4cb910.png)

