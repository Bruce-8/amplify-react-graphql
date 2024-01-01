# Full-Stack Notes Web Application

This project is a cloud-based notes web application using React, AWS Amplify, a GraphQL API configured with an Amazon DynamoDB database, and Amazon S3.

## Features

### Hosting

This app was built and hosted on the AWS global content delivery network (CDN). Through AWS Amplify, this app can be automatically re-deployed through code changes (git commits).

### Authentication

An authentication service was created and deployed using Amplify libraries. Then, the React portion was configured to include this authentication service. The authentication includes two parts:

#### 1. Create Account & Identity Verification

<img src="POCs/Screenshot (155).png" height="300" width="300"/>&nbsp;&nbsp;<img src="POCs/Screenshot (162).png" width="380" height="300"/>

#### 2. Sign In

<img src="POCs/Screenshot (163).png" height="300" width="300"/>

### Database & Storage (CRUD + L)

Deployed a GraphQL API that is backed by the Amazon DynamoDB database and created a storage service using Amazon S3. Combing these features, one can create, fetch, and delete notes as well was optionally upload images. Finally, there is a sign-out option after the user is finished interacting with the app.

#### Create Note

<img src="POCs/Screenshot (164).png" height="350" width="500"/>

#### Fetch Note

Note: This feature is executed upon creating a new note, refreshing the page, or entering the app after a successfull sign in.

<img src="POCs/Screenshot (165).png" height="350" width="500"/>

#### Delete Note

<img src="POCs/Screenshot (166).png" height="350" width="500"/>

## Acknowledgements

This project was created through the guidance of [this tutorial](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/) developed by Amazon Web Services.