# GCP-PHP-CI-CD-USING-YAML
This repository holds a simple yaml script for performing CI/CD for a google cloud platform (GCP), it performs following once a code is pushed to github :
- It checks the branch on which code is pushed.
- Authroises the SSH connection where it get's it credentials from google cloud build service.
- Once accessed the server depending on which the code was pushed.
- It navigates to the application base path, pulls the updated code, cleans the deployment.
- Restarts the servers and done.
- Using this same yaml script we can use composer to update the vendor file i.e. third-party services integrated in our application.
- Even fresh first deployment on the server can be made.

This code uses google cloud build to deploy on the google compute engine, where the necessary credentials and sensitve info is passed by google cloud during runtime.
To use this file you would need to add it to your main code at root level / top most directoary.
