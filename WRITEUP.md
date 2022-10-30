# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

> **In my opinion an app service is an ideal choice for the CMS app.**

Reasons for choosing **App Service**:

- Being a lightweight application, App service should be suitable enough to handle the app
- No special software needs to be installed on the system apart from the Python Runtime
- App Service is a scalable product and hence can be scaled up or down as per traffic
- Ap Service instance Pricing is less compared to a Virtual Machine
- Easy managibility is a big plus for this PaaS 'App Service'
- The option of deploying the app using GIT makes it a faster deployment model

Resons for _NOT_ choosing **Virtual Machine**:

- Being a always on and dedicated product model the operating cost would be much higher
- Maintenace of the machine is a big headache as all OS/framework updates have to done on a regular basis
- Scalabilty is an issue for an VM as it is a complicated as well as more time-consuming approach compared to scaling App service

### Assess app changes that would change your decision.

I might use a **VM** for the app in below mentioned scenarios:

- Federated/Business Rules states that the DB and App should be on the same machine
- It is a mandatory requirement by the client to use a VM
- There is a requirement for special software to be installed on the machine which is not possible in a PaaS environment
- The client wants to use a single machine for hosting multiple apps on a dev/test box
- I might use VM if the load is pretty high and it becomes cheaper and easier to manage one single machine insted of multiple App Service instances
