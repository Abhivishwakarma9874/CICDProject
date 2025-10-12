# CICDProject
This is a CI/CD project. In this project, I used Flask to build a photography website.


How to create a token on GitHub?

Token : 

git remote add origin https://<TOKEN>@github.com/<username>/<repo>.git

git remote set-url origin https://Abhivishwakarma9874:<TOKEN>@github.com/Abhivishwakarma9874/CICDProject.git

PS C:\Users\HP\Documents\photographer\CICDProject> docker build -t abhivishwakarma9874/cicdproject:0.0.1.RELEASE .

PS C:\Users\HP\Documents\photographer\CICDProject> docker container run -d -p 5000:5000 abhivishwakarma9874/cicdproject:0.0.1.RELEASE

PS C:\Users\HP\Documents\photographer\CICDProject> docker container run -d -p 3000:5000 abhivishwakarma9874/cicdproject:0.0.1.RELEASE

docker login 

```cookie
PS C:\Users\HP\Documents\photographer\CICDProject> docker login

USING WEB-BASED LOGIN

i Info → To sign in with credentials on the command line, use 'docker login -u <username>'


Your one-time device confirmation code is: STFT-FFXF
Press ENTER to open your browser or submit your device code here: https://login.docker.com/activate

Waiting for authentication in the browser…
docker login
Login Succeeded
PS C:\Users\HP\Documents\photographer\CICDProject> 
```
PS C:\Users\HP\Documents\photographer\CICDProject> docker push abhivishwakarma9874/cicdproject:0.0.1.RELEASE

