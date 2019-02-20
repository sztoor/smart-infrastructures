# smart-infrastructures
One model for one question, making the e-infrastructures smart


## Steps to configure the environment

Note: The containers are based on TensorFlow base containers. 

1 - Install docker. https://docs.docker.com/install/, https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04

2 - Pull question container.  

```docker pull salmantoor/smart-infrastructures:question-1```
 
3 - Create following three directories:

   -  ```smart-infra```
   -  ```smart-infra/input-data```
   -  ```smart-infra/input-data```
   
4 - Goto smart-infra directory.

5 - Place all input files in the ```input-data``` directory. 

6 - Start the container with the following command: 

```docker run  -it -v /Users/salmantoor/smart-infra/input-data:/smart-infra/input-data  -w /smart-infra smart-infra/question-1 python model.py```

7 - The ```output-data``` directory will contain the results of the run. (Need some work .. )

