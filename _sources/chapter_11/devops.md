# Chapter 11: DevOps

DevOps is about integrating developer and operations teams to improve
collaboration and productivity through automating 
a system's workflows (infrastructure, deployment process etc.).

The purpose of this guide is to introduce students to DevOps and
demonstrate how it can help streamline your development workflow.

## Before DevOps

There are two teams that are core to delivering functional software:

- *Developer teams:* develop, build, and test features.
- *Operations teams:* manage the change management, security,
    deployment, monitoring, and feedback.

The development and operations teams previously worked in isolation -
the developer team worked on the product while the operations team
handled the release. This led to a lot of problems when it came to when
it came to integrate code and manage the release.

```{figure} resources/devops.jpg
---
name: devops
---
{cite:p}`Accenture`
```

## DevOps Explained

DevOps aims to break down these silos by enabling developer and
operations teams to work together. This increases collaboration and
allows teams to manage releases by using automated workflows.

### Terminology

- *Automation:* using technology to perform a task in a reproducible
    way, such that feedback is provided on the process itself and
    minimal human intervention is required.
- *DevOps pipeline:* set of automated processes. Includes continuous
    integration, continuous delivery/deployment, etc.

## CI/CD

### What Is CI/CD?

CI/CD refers to continuous integration and continuous
delivery/deployment. These are a set of practices that allow teams to
deliver software to a production environment without having to rely on
cumbersome manual processes. Through automating parts of the release
process, CI/CD allows developers to make quicker releases.

### Why CI/CD?

1. Fast: the time taken for releases are significantly reduced through
    automating the workflow.
2. Simple: the process of integrating code becomes much simpler
3. Fewer errors: less intervention from developers is required which
    reduces the chance for human error
4. Isolated failures: immediate feedback provided as to which step in
    the pipeline has failed

There are several CI/CD providers, but we recommend using GitHub Actions
as it is free and easy to use. When you have created your repository,
refer to our CI/CD guide on how to get started with GitHub Actions.

### CI/CD Terminology

- Continuous Integration: Integrating your code changes back to your
    main branch. Changes are checked by automatically building, testing
    code.
- Continuous Delivery: Extension of CI. Automates the release process
    so that you can deploy the application at any time.
- Continuous Deployment: Extension of continuous delivery. Automate
    deployment to production environment if all other stages are
    successful.

```{figure} resources/cicd.png
---
name: cicd
---
{cite:p}`AtlassianCICD`
```

## DevOps Pipeline

Teams should use CI/CD within their projects, using either continuous
delivery or deployment. CI/CD is achieved using pipelines.

### Creating Your Pipeline

Pipelines refer to a set of steps executed when some condition is met.
Often, teams will customise their pipelines to be triggered on pull
requests. This means, when a developer creates a pull request to merge
code changes from their branch to the main branch, the pipeline will
automatically run the set of steps specified.

Ordinarily, developers perform several checks before merging any code.
You want to make sure your project builds successfully, the code follows
any formatting conventions, and that all the test cases written still
pass. When creating your pipeline, these kinds of checks are written as
steps that you want to be executed on your given condition. As such,
teams should ensure that when they create their pipeline, they should
include the following steps:

- install dependencies and build
- format
- run
- test

### An Example CI/CD Workflow

Let us consider an example of how this may look. Once you have your
pipeline, the workflow is simple. Consider the case where your pipeline
is triggered on pull requests. A team member makes a pull request from
their own branch, dev/authentication, into the main branch, main. This
will trigger the pipeline to execute, and it will sequentially build,
format, run, and test as stipulated in the pipeline. If any step fails,
it will indicate which step failed and developers can even inspect the
logs to find why.

Once all the steps successfully complete, the pipeline will indicate
that the code has passed all its checks. This will then allow other
developers to review the code themselves, before approving the pull
request. Once the code is accepted, a developer can merge the code from
dev/authentication into main. From here, you can either have a separate
pipeline set up to handle the deployment process or allow your
deployment provider to deploy from the main branch.

This workflow is shown below:

```{figure} resources/example_workflow.png
---
name: example_workflow
---
{cite:p}`GitLab`
```

## Deployment

Deployment refers to the set of steps that are required to *make your
application accessible to the public*. There are three types of
deployment tools available:

| SaaS                           | PaaS                                                                          | IaaS                                                  |
|--------------------------------|-------------------------------------------------------------------------------|-------------------------------------------------------|
| Software as a service.         | Platform as a service.                                                        | Infrastructure as a service.                          |
| The vendor manages everything. | Vendor manages architecture, but you develop the application and manage data. | You manage the infrastructure, data, and application. |
|                                |                                                                               |                                                       |

```{note}
For this subject, we highly recommend you use PaaS deployment tools
as this allows you to focus on building the application.
```

## PaaS

### PaaS Providers

- [Heroku](https://www.heroku.com/)
- [AWS elastic beanstalk](https://aws.amazon.com/elasticbeanstalk/)
- [Netlify](https://www.netlify.com/)
- [Microsoft Azure Cloud Services](https://azure.microsoft.com/en-us/services/cloud-services/)
- [GitHub Pages](https://pages.github.com/)

### PaaS Deployment

Deployment could be achieved in several ways and is up to your team to
choose a deployment strategy:

- Configure PaaS deployment tool to deploy automatically from your
    main branch.
- Specify the deployment as a step in your pipeline.

:::{admonition} Extra Resources
:class: tip

- [Short summary of CI/CD](https://www.youtube.com/watch?v=scEDHsr3APg&ab_channel=Fireship)
- [PaaS vs SaaS vs IaaS](https://www.bmc.com/blogs/saas-vs-paas-vs-iaas-whats-the-difference-and-how-to-choose/)
:::
