# Executable Renovate-tutorial

## Introduction
Renovate is a dependency manager and its main use is to monitor all dependencies in a project and automatically update them according to your chosen preferences. For instance, Renovate bot will automatically crate pull requests whenever dependencies need updating. Renovate supports a wealth of languages and is highly customizable. There are multiple options on how to set up and use Renovate. It is easily available if you are hosted at Github or Azure DevOps. For platforms such as Bitbucket Cloud, Bitbucket Server, Gitea and GitLab, Renovate can be used by self-hosting it.

This tutorial will provide a breif introduction to the tool and how to set up Renovate bot for an example node application hosted on Github.

## Table of Contents
1. Preparation
2. Instructions

## Preparation
To complete this tutorial you will need a Github account and a web-browser.

## Instructions

1. The example project we are going to use is a simple web server that listens to clients that connect to <http://localhost:3000>. When a client connects to the server, then the server sends the message "Hello World!" as a response. The example project can be found here <https://github.com/Sebberh/GenericNode>. For more details about the example project, check its README. Moving on to the first step of this tutorial, navigate to <https://github.com/Sebberh/GenericNode>

2. Fork the repository
![](images/2.png)

3. Navigate to <https://github.com/apps/renovate> and click the Install button
![](images/3.png)

4. Set repository to either "All repositories" or just select the fork.
![](images/4.png)

5. Click Install

6. Click Activate now and sign in with Github
![](images/6a.png)

7. Go to your Fork

8. Go to Pull requests and open the pull request named Configure renovate
![](images/8.png)<br/>
It should look something like this:
![](images/8b.png)
9. Read through the configuration summary and consult the official documentation. If there are anything you don't understand(https://docs.renovatebot.com/).

10. Merge the pull request to enable Renovate on your Fork

11. Check the list of pull request again to find an automatically created pull request updating the version of node in the project.
![](images/11.png)
12. Merge the pull request to update.

13. The configuration can be found in  renovate.json, explore the depths of configuration available at <https://docs.renovatebot.com/configuration-options/> at your own leisure.
