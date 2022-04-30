# Documentation of project 9
## Step 1
1. I created an aws ec2 ubuntu server and named it jenkins-server
  
  ![ubuntu](images/image1.PNG)

2. I installed jdk

  `sudo apt update`
  `sudo apt install default-jdk-headless`
  `wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -`
`sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \`
    `/etc/apt/sources.list.d/jenkins.list'`
`sudo apt update`
`sudo apt-get install jenkins`

   ![ubuntu](images/image2.PNG)
   ![ubuntu](images/image3.PNG)
   ![ubuntu](images/image4.PNG)

3. I ensured jenkins was up and running
   
   `sudo systemctl status jenkins`
   ![ubuntu](images/image5.PNG)

4.  I opened TCP port 8080 on my security group
    
5.  I confirmed the initial jenkins setup on my browser

   ![ubuntu](images/image6.PNG)

6. Then I retrieved password from the server
   ![ubuntu](images/image7.PNG)

7.  I installed suggested plugins
   ![ubuntu](images/image8.PNG)
   ![ubuntu](images/image9.PNG)
   ![ubuntu](images/image10.PNG)

8. My setup was ready
    ![ubuntu](images/image11.PNG)
    ![ubuntu](images/image12.PNG)

## Step 2
1. I enabled webhooks in my github repository
   ![ubuntu](images/image13.PNG)

2. I created a 'freestyle project' in my jenkins web console
   ![ubuntu](images/image14.PNG)

 3. I configured my jenkins freestyle project
    ![ubuntu](images/image15.PNG)

4.  I saved the configuration and tried to run the build
    ![ubuntu](images/image16.PNG)
    ![ubuntu](images/image17.PNG)
    
5. I configured 'post-build actions to archive the files'
    
    ![ubuntu](images/image18.PNG)

## Step 3
1. So as to install publish over ssh, I clicked on 'manage jenkins' on the dashboard
     ![ubuntu](images/image19.PNG)

2. Then I clicked on plugin Manager
      ![ubuntu](images/image20.PNG)

3. It was installed successfully

     ![ubuntu](images/image21.PNG)

4. Then, I configured it

   ![ubuntu](images/image22.PNG)
   ![ubuntu](images/image23.PNG)

5. I tested the configuration and it was successful

    ![ubuntu](images/image24.PNG)

6. I confirmed it on my windows terminal and it worked

    ![ubuntu](images/image25.PNG)

