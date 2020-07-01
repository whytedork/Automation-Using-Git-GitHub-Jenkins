LinkedIn Post Link : 

https://www.linkedin.com/posts/whytedork_session8abrdevopsabrtask-righteducation-rightmentor-activity-6664042084539998208-M1bT/

# Problem Statement :
+ create 3 jobs in jenkins named as job1, job2 , job3
+ create a git repository with two branches
1.master(default)
2.dev1

+ There are two docker containers containing webserver running in background
* First for testing
* Second for Client / Production

+ use hooks for automatic integration and automatic deployment

+ when we commit in dev1 branch then automatically push data on github and run all jobs along with deploying docker conatiners

+ branch dev1 is associated with job2 which will do testing and deploy docker container for testing

+ branch master is associated with job1 which will do continuous deployment for client and deploy docker container using tunneling (ngrok)

+ job 3 : if testing is successful then jenkins merge the dev branch to master branch and trigger job1
+ also send email to client when deployment is successful(check comment box)
