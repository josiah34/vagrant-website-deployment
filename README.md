# vagrant-website-deployment

<ins>**Overview**</ins>

This repository is to document my project where I use vagrant to automate the provisioning of a linux virtual machine (Centos 7) and the deployment of a website template. I will do it manually first then destroy the vm and automate the entire process within the provisioning stage. Security is out of scope for this project as this is purely for learning purposes.  

<ins>**Website Template**</ins>

This is the template I used but any template on the site `tooplate.com` will work.

[Crispy Kitchen](https://www.tooplate.com/view/2129-crispy-kitchen)
![template](https://user-images.githubusercontent.com/25124463/215350476-8901162c-6ff1-4e44-86bc-d32cae937995.jpg)



## Steps

1. The first thing I will do is create a new directory within my Vagrant directory that I will name `crispy-kitchen`
   ```
   mkdir crispy-kitchen 
   ```
   ![mkdir-crispy-kitchen](https://user-images.githubusercontent.com/25124463/215351255-d3c0804b-797f-4406-88bf-c96f87348496.jpg)

2. Next I'll change directory to the newly created `crispy-kitchen`. 
   ```
   cd crispy-kitchen
   ```
3. Now we have to initialize this directory as a vagrant environment with the image from vagrant cloud that we want to use. I will be using `geerlingguy/centos7`
   
   ```
   vagrant init geerlingguy/centos7
   ```
 4. This will download the vagrant file. We are now ready to issue the `vagrant up` command. Before that we will edit a few things in the Vagrant File. You can use any text editor to do this. I use vim for powershell.
      ```
      vim Vagrantfile
      ```
 5.  We have to uncomment out the following lines `config.vm.network "private_network", ip: "192.168.33.10"` and `config.vm.network "public_network`. Save the file and exit.
     ![remove-comments](https://user-images.githubusercontent.com/25124463/215352343-ad0a96bc-aa90-4f89-a0c7-0af36539e8dc.jpg)
     
 6.
   



