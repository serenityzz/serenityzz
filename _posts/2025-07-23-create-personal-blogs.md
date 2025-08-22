---
title: "Create a personal website"
date: 2025-07-23
tags: 
- technical writing
- GitHub
---

📑

Technical writers are often asked to provide writing samples to showcase their skills. Rather than storing them locally, creating a personal site for your portfolio makes it accessible from anywhere, at any time. One easy way to do so is by using GitHub Pages to create a static website from a GitHub repository. 

## Introduction

GitHub Pages is a feature of GitHub that lets you host a static website directly from a GitHub repository. It works by connecting your GitHub repository to a website. When you upload content (such as Markdown or HTML files) to your repository, GitHub Pages automatically generates a website. GitHub Pages is ideal for hosting personal blogs and websites to showcase portfolios and project experience. 

GitHub Pages uses Jekyll, a static site generator, to build your website. You can either create your own site from scratch or use pre-built Jekyll themes to simplify the process. This topic provides instructions on creating a GitHub Pages website using a pre-built Jekyll theme.

## Before you start

Before you start, familiarize yourself with the following:

- Markdown or HTML basics. GitHub Pages supports both HTML and Markdown files. We recommend using Markdown as it is easier to learn. To get started with Markdown, see the [Markdown syntax guide]([Basic Syntax | Markdown Guide](https://www.markdownguide.org/basic-syntax/)).

- Basic Git concepts. To work with GitHub effectively, it is important to understand basic Git concepts:
  
  - **Branches:** A branch is an isolated working copy of your repository. In GitHub it is recommeded to create a branch to make and test changes, and then merge the changes into the main branch.
  
  - **Pull requests:** A pull request (PR) refers to merging changes from one branch to another. In GitHub Pages, you may create a pull request to merge changes from a branch of a repository to the main branch. 

## Create a GitHub Pages website

The easiest way to create a GitHub Pages website is by forking (copying) a Jekyll theme repository. Jekyll themes provide pre-configured layouts and styles for a website. In GitHub there is a variety of pre-built Jekyll themes that you can use to quickly build your website. This section provides the step-by-step instructions.

### To create a GitHub Pages website by copying a Jekyll repository:

1. Log in to [GitHub](https://github.com/) or sign up if you don't have an account.

2. Go to the [public Jekyll themes](https://github.com/topics/jekyll-theme) page, browse the available Jekyll themes, and select one for your site.

3. Open the target Jekyll theme repository and click **Fork** at top right. 
   
   > **Tip:** Fork means copy. Forking a repositiory lets you make a copy of the repository to your GitHub account and make the changes you want without affecting the original repository. 

4. On the **Create a new fork** page, set the following fields:
   
   - **Owner:** This is auto-filled with your GitHub username.
   
   - **Repository name:** Rename the repositiory to `YOURUSERNAME.github.io`, where `YOURUSERNAME` must be your GitHub username.  
     
     > **Note:** It's important to use your GitHub username, so that GitHub can recognize it and create a website for your repository.

5. Click **Create fork** to copy the Jekyll theme repository to your GitHub account.

6. Open the forked repository on your GitHub account, click **Settings** at the top and then select **Pages** in the left pane. 

7. In the **Build and deploy** area, set the following fields:
   
   - **Source:** Select **Deploy from a branch.**
   
   - **Branch:** Select **`main`** or **`master`**. 

8. Click **Save** to enable GitHub Pages site for your repository. You can now add content files to the repository. 

## Add content to your website

After creating and setting up a GitHub Pages website, you can now add content to it. 

### To add content to your website:

1. Open your website repository and create a branch for it. 
   
   > **Tip:** A branch is an isolated working copy of your repository. It is recommended that you make and test changes in a branch, then merge them into the main branch using a pull request.
   
   a. At the top left, locate the branch selector dropdown (it usually displays **`main`** or **`master`**).
   
   b. Click the dropdown and then in the field that appears, type the name of your new branch, for example, `my-pages`. 

2. Select the new branch and then navigate to the `README.md` file. The `README.md` file contains instructions on how to configure settings and manage content for your website. 

3. Follow the instructions in the `README.md` file to configure your website and add content files, and then click **Commit changes** to save your edit. 
   
   > **Tip:** In order for the Jekyll theme to process the content files and turn them into a functional website, you must use the specified format for the content files and place them under the designated folder. For details, follow the instructions in the `README.md` file.

4. When you have added content files for your website, review the files in the branch to make sure everything works fine, and then merge the chanages to the main branch.
   
   a. Click **Pull requests** at the top.
   
   b. Under **Comparing changes**, select the **base branch** (usually `main` or `master`) and the **compare branch** (the branch with your changes).
   
   c. GitHub displays the changes you have made between the two branches. Review them to ensure everything looks good.
   
   d. Click **Create pull request** and then click **Merge** to merge your changes from the working branch to the main branch. 

5. Wait for a few minutes for the content to be published. You can view your live website at `http(s)://<yourusername>.github.io/<yourusername>`.
