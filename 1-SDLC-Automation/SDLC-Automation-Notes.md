# SDLC Automation Notes

This document contains my notes from various resources for the SDLC Automation section of the AWS Certified DevOps Engineer – Professional exam.

## AWS CodePipeline User Guide
**URL**: [AWS CodePipeline User Guide](https://docs.aws.amazon.com/codepipeline/latest/userguide/welcome.html)

**Key Takeaways**:

- Automated Release Process: CodePipeline automates the entire release process, from the source repository through build, test, and deployment phases. It allows for manual approval actions in any stage except the Source stage, offering control over when and how releases happen, across single or multiple instances.

- Consistent Release Process: It enables the definition of a consistent set of steps for every code change, ensuring each stage of the release meets your criteria.

- Faster Delivery and Improved Quality: Automating the release process allows for incremental testing and faster release of new features, enhancing both the speed and quality of deliveries.

- Integration with Favorite Tools: CodePipeline supports integration with existing source, build, and deployment tools. A full list of compatible AWS services and third-party tools is available in the CodePipeline documentation.

- Real-Time Progress Monitoring: Provides a real-time view of pipeline status, including alerts, failure details, source revision information, and the ability to retry failed stages or manually rerun pipelines.

- Pipeline History Tracking: Offers detailed insights into pipeline executions, including start and end times, duration, and execution IDs.

**AWS CodePipeline Concepts Summary:**

**Pipelines**
- Workflow construct describing the release process of software changes.
- Composed of a series of stages.

**Stages**
- Logical units for isolating environments and limiting concurrent changes.
- Contain actions performed on artifacts like source code.
- Examples: build stage (source code build and testing) and deployment stage (code deployment to runtime environments).
- Stages consist of serial or parallel actions.

**Actions**
- Operations performed on application code at specified pipeline points.
- Types include source, build, test, deploy, approval, and invoke.
- Can run in series or parallel.

**Pipeline Executions**
- Unique set of changes released by a pipeline, each with its own ID.
- Corresponds to changes like a merged commit or manual latest commit release.
- Stages process one execution at a time, locking the stage during processing.
- Valid statuses: InProgress, Stopping, Stopped, Succeeded, Superseded, Failed.

**Stopped Executions**
- Can be stopped manually, showing 'Stopping' then 'Stopped' status.
- Two stopping options: stop and wait, stop and abandon.

**Failed Executions**
- Stop and don't traverse the entire pipeline if they fail.
- Unlock the stage, allowing newer executions to proceed.

**Superseded Executions**
- Newer executions can replace older ones already running through the pipeline.
- Superseded executions stop and don't traverse the entire pipeline.

**Stage Executions**
- Process of completing all actions within a stage.
- Valid statuses: InProgress, Stopping, Stopped, Succeeded, Failed.

**Action Executions**
- Completion of configured actions on designated artifacts.
- Valid statuses: InProgress, Abandoned, Succeeded, Failed.

**Artifacts**
- Data worked on by pipeline actions, like source code and built applications.
- Can be input or output artifacts.

**Source Revisions**
- Versions of source changes triggering pipeline executions.
- Executions process the specific source revision that triggered them.


## AWS CodeBuild Documentation
- **URL**: [AWS CodeBuild Documentation](https://docs.aws.amazon.com/codebuild/latest/userguide/welcome.html)
- **Key Takeaways**:
  - 


## AWS CodeDeploy Documentation
- **URL**: [AWS CodeDeploy Documentation](https://docs.aws.amazon.com/codedeploy/latest/userguide/welcome.html)
- **Key Takeaways**:
  - 

## Practicing Continuous Integration and Continuous Deployment on AWS
- **URL**: [Continuous Integration and Deployment Whitepaper](https://aws.amazon.com/whitepapers/practicing-continuous-integration-continuous-deployment-using-aws/)
- **Key Takeaways**:
  - 

## Infrastructure as Code Whitepaper
- **URL**: [Infrastructure as Code Whitepaper](https://d1.awsstatic.com/whitepapers/DevOps/infrastructure-as-code.pdf)
- **Key Takeaways**:
  - 

## External Articles and Blog Posts

### DevOps on AWS Blog
- **URL**: [DevOps on AWS Blog](https://aws.amazon.com/blogs/devops/)
- **Key Takeaways**:
  - 

### Introducing DevOps in an Enterprise Environment
- **URL**: [Introducing DevOps in an Enterprise Environment](https://www.thoughtworks.com/insights/blog/introducing-devops-enterprise-environment)
- **Key Takeaways**:
  - 

### Using Containers for Continuous Deployment
- **URL**: [Using Containers for Continuous Deployment](https://www.infoq.com/articles/Continuous-Deployment-Containers/)
- **Key Takeaways**:
  - 

### Microservices on AWS Blog
- **URL**: [Microservices on AWS Blog](https://aws.amazon.com/blogs/compute/microservices-on-aws/)
- **Key Takeaways**:
  - 

## Forums and Communities

### AWS Developer Forums
- **URL**: [AWS Developer Forums](https://forums.aws.amazon.com/)
- **Key Takeaways**:
  - 

### Stack Overflow
- **URL**: [Stack Overflow](https://stackoverflow.com/questions/tagged/aws-codepipeline+aws-codecommit+aws-codedeploy)
- **Key Takeaways**:
  - 

