---
title: "Create a personal site with GitHub Pages"
date: 2025-07-23
tags: 
- technical writing
- GitHub
---

📑<br>

Technical writers are often asked to provide writing samples to showcase their skills. Rather than storing them locally, creating a personal website for your portfolio makes it accessible from anywhere, at any time. One easy way to create a peronal website is to create a GitHub Pages site from a GitHub repository. This topic walks you through the process.<br>

## Introduction to GitHub Pages website

GitHub Pages is static site generation service provided by GitHub, which is a web-based platform for software development teams to store, manage, and track changes to code and documents using Git, a version control system. <br>

You create a repository (you can think of a repoisitory as a project) on GitHub to store and organize files for your website. The built-in GitHub Pages feature uses a static site generator to take files from the GitHub repository and turn them into a static website. The GitHub Pages supports the **Jeklyll** static site generator or a custom one. We recommend using Jekyll, which is with built-in support for GitHub Pages. Jekyll offers templates, called themes, that provide pre-configured layouts and styles for a website. You can easily integrate one Jekyll theme with your GitHub repository to create a website without designing everything from scratch. <br>

## Before you start

Before you start, familiarize yourself with the following:

- Markdown or HTML basics. GitHub Pages supports both HTML and Markdown files. We recommend using Markdown, as it is easier to learn. To get started, see the [Markdown syntax guide]([Basic Syntax | Markdown Guide](https://www.markdownguide.org/basic-syntax/)).

- Basic Git concepts. To work with GitHub effectively, it is important to understand basic Git concepts, such as pull requests, push requests, merge requests, and branches.

## Create a GitHub Pages website

There are several methods to create a GitHub Pages website. The simplest one is to copy a Jekyll repository to your GitHub account and manage content in the copied repository. This section provides the step-by-step instructions.

### To create a GitHub Pages website by copying a Jekyll repository:

1. Log in to [GitHub](https://github.com/) or sign up if you don't have an account.

2. Go to the [public Jekyll themes](https://github.com/topics/jekyll-theme) page, browse the available Jekyll themes, and select one for your site.

3. Click the target Jekyll theme to open its repository and click **Fork** at the top right of the page. 
   
   > **Tip:** Fork means copy. Forking a repositiory lets you make a copy of a respository to your GitHub account and make the changes you want without affecting the original repository. 

4. On the **Create a new fork** page, set the following fields:
   
   - **Owner:** This is auto-filled with your GitHub username.
   
   - **Repository name:** Rename the repositiory to `YOURUSERNAME.github.io`, where `YOURUSERNAME` must be your GitHub username.  
     
     > **Note:** It's important to use your GitHub username, so that GitHub can recognize it and create a website for your repository.

5. Click **Create fork** to make a copy of the Jekyll repository to your GitHub account.

6. Open the forked repository on your GitHub account, click **Settings** at the top and then select **Pages** in the left pane. 

7. In the **Build and deploy** area, set the following fields:
   
   - **Source:** Select **Deploy from a branch.**
   
   - **Branch:** Select the branch that contains the files to publish. It is recommended to select the main (usually **`main`** or **`master`**) branch. 

8. A GitHub Pages site is created for your GitHub Repository. You can then add content to your website by adding files to your GitHub repository. 

## Add content to your website

After creating and setting up your GitHub Pages website, you can now add content to it. 

### To add content to your website:

1. Open your website repository on your GitHub account and create a branch for it. 
   
   > **Tip:** A branch is an isolated working copy of your repository. We recommend making and testing changes in a branch, then merging them into the main branch using a pull request.
   
   a. At the top left, locate the branch selector dropdown (it usually displays **`main`** or **`master`**).
   
   b. Click the dropdown and then in the field that appears, type the name of your new branch, for example, `my-pages`. 

2. Select the new branch and then open the `README.md` file. The `README.md` file contains instructions on how to configure settings and manage content for your website. 

3. Follow the instructions in the `README.md` file to configure your website and add content files, and then click **Commit changes** to save your changes. 
   
   > **Tip:** In order for the Jekyll theme to process the content files and turn them into a functional website, use the specified format for the content files and place them under the designated folder. For details, follow the instructions in the `README.md` file.

4. When you have added content files for your website, review the files in the branch to make sure everything works fine, and then merge the chanages to the main branch.
   
   a. Click **Pull requests** at the top.
   
   b. Under **Comparing changes**, select the **base branch** (usually `main` or `master`) and the **compare branch** (the branch with your changes).
   
   c. GitHub displays the changes you have made between the two branches. Review them to ensure everything looks good.
   
   d. Click **Create pull request** and then click **Merge** to merge your changes from the working copy to the main repository.

5. Wait for a few minutes for the content to be published. You can view your website at `http(s)://<yourusername>.github.io/<yourusername>`.
