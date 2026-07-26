# Zinnia

- an enterprise operations management platform
- in English: code that helps a team organize work, people, and equipment in one place
- named after the <a href="https://www.youtube.com/watch?v=IWqJMne8xbU">fourth track</a> on Clairo's 2021 album <i>Sling</i>
- Zinnia is like Jira mixed with ServiceNow. People can create work orders, assign them, track assets, and watch updates happen live.

## Tech stack
- C# to write the backend programs
- ASP.NET Core to turn those programs into web APIs
- React to build the website people use
- TypeScript to make the website code easier to maintain
- PostgreSQL to remember work orders, assets, and users
- SignalR to instantly show updates without refreshing the page
- Docker to package everything so it runs the same everywhere
- AWS ECS to run the packaged application in the cloud
- Terraform to create the cloud infrastructure automatically
- GitHub Actions to automatically test and deploy new code
- CloudWatch to monitor the application and catch problems

## Mental model
```
Employee
    │
    ▼
React website
    │
    ▼
ASP.NET Core API
    │
    ▼
PostgreSQL

SignalR keeps everyone's screens updated
Docker packages everything
AWS ECS runs everything
Terraform builds the AWS infrastructure
GitHub Actions deploys everything
CloudWatch watches everything
```
