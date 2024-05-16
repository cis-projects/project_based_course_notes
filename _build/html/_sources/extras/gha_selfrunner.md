# GitHub Actions: Self-Hosted Runner

## Introduction to Using Local Self-Hosted Runners for GitHub Actions

In our university's tech programs, collaboration and resource sharing are essential. As we advance in our courses and projects, it's important to be mindful of the resources available to us. Currently, our GitHub organization is allocated **2000 minutes per month** for GitHub Actions, shared among all students. Given this limitation, it's vital for each of us to adopt practices that help conserve these valuable minutes.

### Why Use Local Self-Hosted Runners?

Local self-hosted runners provide an excellent solution for running GitHub Actions without consuming our shared minutes. This approach allows students to test and develop projects locally, preserving our GitHub minutes for critical stages of the project, such as final deployments at the end of development sprints.

By setting up a self-hosted runner on your personal machine, you can execute all necessary actions and checks on your projects without tapping into the shared pool of minutes. This not only ensures that resources are available when truly needed but also promotes a more responsible use of our collective assets.

### How This Benefits You

- **Maximise Resources:** Allows more extensive testing and integration processes without the fear of depleting our action minutes.
- **Faster Iterations:** Local runners often provide quicker feedback loops for your project builds and tests.
- **Enhanced Learning:** Gain hands-on experience with an importante aspect of modern DevOps practices by managing your own CI/CD pipelines.

Adopting local self-hosted runners is more than a convenience—it's a necessity for ensuring that all students have equal access to our limited resources when they need them most. Let's all do our part to make the most of what we have. Follow the setup guide below to get started with your own self-hosted runner.


## Local Self-Hosted Runners

The tutorial below was developed by team SI-Koala (COMP90082 - 2024 - SM1: Rishabh Srivastava, Vijay Narayan Venkatesh, Edwin Zhu, Saraubh Unmesh Zingade, Akash Renuka Ashok). This documentation is to assist anyone looking to set up a self-hosted runner for their team. It is straightforward and can make your automation much more affordable.

### How to Setup Self-Hosted Runners

To conserve GitHub Actions compute minutes, we run GitHub Actions on our local machines instead of using larger GitHub-hosted runners or standard GitHub-hosted runners. This has minimal impacts on how developers utilize DevOps.

### Steps to Setup:

1. Navigate in your repository to `Settings -> Code and Automation -> Actions -> Runners`.
2. Click on `New self-hosted runner`.
3. Select your laptop's configuration (OS: macOS/Linux/Windows, Arch: x64, ARM64, ARM) and follow the steps provided in the UI.
4. It is advisable to create an `actions-runner` folder in the root directory.

### Installation Steps:

- **Download:** Downloads the GitHub Actions package to your machine and extracts the installer.
- **Configure:** Using the provided token, you authorize the runner to access the repository.

### More About Configuration:

- Most setup steps can retain default values.
- Ensure the name of the runner includes the user's name (e.g., `Rishabhs-MacBook-Pro`).
- **Labels:** Labels are crucial in this setup. By default, you will get values like `self-hosted, macOS`, etc. You can add more labels, which can be used in your workflows to filter which runner to use for the build.

### Example:

A runner can have a label `android`, and you can specify `runs-on: android` in your workflows for Android builds.

### Final Steps:

1. Make sure the runner is running on your machine using `./run.sh` and do not exit the terminal.
2. If you go to `Repository -> Settings -> Code and Automation -> Actions -> Runners`, you should be able to see the newly created runner in status `Idle`, indicating it is ready to start picking up your GitHub Actions jobs. As long as your workflow uses the correct labels (`self-hosted, macOS`, etc.), it should get picked up.

Container based plugins were having a problem with this approach. In this case, please try and setup a Linux runner on your macOs. The commands for linux should run fine on macOS as well. 

Happy days! 🚀 
