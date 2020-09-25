**hello_jenkins**     

This simple exercise is designed to introduce you to Jenkins and continuous integration.     

**Overview**          
1. Fork the repo.           
2. Set up job in Jenkins to connect to your repository and build C hello.c.       
3. Set up build status badge.          
4. Set up second job to run the program after build completes.           

**Prerequisites**          
A Jenkins server is needed in order to complete the exercise. One option is local virtualization using Docker or a virtual machine.       

**Setting up a Job in Jenkins**                  

Navtigate to Jenkins server.
1. Click *New Item*.       
2. Enter a name for your project, click *hello* Project, then OK.      
3. Note: Please do not include a space.           
4. Name this something unique so there are no collisions.             
5. Set up *Source Code Management*.            
6. Select *git*.           
7. Enter the URL to your git repository             
8. Setting up *Build Triggers*.                 
9. Select *Poll SCM*.                    
10. Set up cron job by putting in H/2 * * * *.            
11. Set up *Build*.                  
12. Add build step *Execute Shell*.            
13. Enter *make* (This will run the Makefile).            
14. Click *Save*.            

