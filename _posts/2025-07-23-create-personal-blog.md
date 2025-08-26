---
title: "Create a personal website"
date: 2025-07-23
tags: 
- technical writing
- GitHub
---

📑
Technical writers are often asked to provide writing samples to showcase their skills. Rather than storing them locally, creating a personal site for your portfolio makes it accessible from anywhere, at any time. One way to do so is by using GitHub Pages to create a static website from a GitHub repository. 

## Introduction to GitHub Pages

GitHub Pages is a GitHub feature that lets you host a static website directly from a repository. When you add content such as Markdown or HTML files, GitHub Pages automatically builds and publishes the site. You can use GitHub Pages to host personal blogs, portfolios, or resumes. 

GitHub Pages uses Jekyll, a static site generator, to create the site. To design your site, you can either choose from a variety of Jekyll themes with predefined layouts and styles, or create one from scratch with a custom site generator. 

This topic describes how to build a site by using a Jekyll theme.

## Before you start

Before you start, familiarize yourself with the following:

- **Markdown or HTML basics.** GitHub Pages supports both HTML and Markdown files. We recommend using Markdown as it is easier to learn. To get started with Markdown, see the [Markdown syntax guide]([Basic Syntax | Markdown Guide](https://www.markdownguide.org/basic-syntax/)).

- **Basic Git concepts.** To work with GitHub effectively, it is helpful to understand these basic Git concepts: 
  
  - **Branches:** A branch is an isolated working copy of your repository. In GitHub it is recommeded to create a branch to make and test changes, and then merge the changes into the main branch.
  
  - **Pull requests:** A pull request (PR) refers to merging changes from one branch to another. In GitHub Pages, you may create a pull request to merge changes from a branch of a repository to the main branch.

## Create a GitHub Pages site

This section describes how to create a GitHub Pages site by using a Jekyll theme. A Jekyll theme defines the layout and style of your site. GitHub Pages provides various Jekyll themes that you can select to quickly build your site. 

### To create a site using a Jekyll theme:

1. Log in to [GitHub](https://github.com/) or sign up if you don't have an account.

2. Go to the [public Jekyll themes](https://github.com/topics/jekyll-theme) page, browse the available themes, and select one for your site.

3. Open the target theme's repository and click **Fork** at top right. 
   
   ![Alt text](/assets/images/posts/example.png)
   
   **Tip:** Forking creates a copy of a repository to your GitHub account. You can then add your site content by adding files to the copied repository. This is the simplest way to start using a Jekyll theme.

4. On the **Create a new fork** page, set the following fields:
   
   - **Owner:** This is auto-filled with your GitHub username.
   
   - **Repository name:** Rename the repositiory to `YOURUSERNAME.github.io`, where `YOURUSERNAME` must be your GitHub username.  
     
     > **Note:** It's important to use your GitHub username, so that GitHub Pages can recognize it and create a website for your repository.

5. Click **Create fork** to copy the theme's repository to your GitHub account.

6. Open the copied repository on your GitHub account, click **Settings** at the top and then select **Pages** in the left pane. ![Alt text](/assets/images/posts/example.png)

7. In the **Build and deploy** area, set the following fields:
   
   - **Source:** Select **Deploy from a branch.**
   
   - **Branch:** Select **`main`** or **`master`**. 

8. Click **Save** to enable GitHub Pages for your repository. 
   
   When you add content files and commit your changes, GitHub Pages automatically generates and publishes the site. 

## Add content to your site

After creating and setting up the GitHub Pages site, you can now add content to it. 

### To add content to your site:

1. Open your website repository and create a branch for it. 
   
   > **Tip:** A branch is an isolated working copy of your repository. It is recommended that you make and test changes in a branch and then merge them into the main branch using a pull request.
   
   a. At the top left, locate the branch selector dropdown (it usually displays **`main`** or **`master`**).
   
   b. Click the dropdown and then in the field that appears, type the name of your new branch, for example, `my-pages`. 

2. Select the new branch and then open the `README.md` file. The `README.md` file contains instructions on how to configure settings and manage content for the site. 

3. Follow the instructions in the `README.md` file to configure the site and add content files, and then click **Commit changes** to save your changes. 
   
   > **Tip:** In order for the Jekyll theme to process the content files and turn them into a functional site, you must use the specified format for the content files and place content files under the designated folder. For details, follow the instructions in the `README.md` file.

4. When you have added content files for your website, review the files in the branch to make sure everything works fine, and then merge the chanages to the main branch.
   
   a. Click **Pull requests** at the top.
   
   b. Under **Comparing changes**, select the **base branch** (usually `main` or `master`) and the **compare branch** (the branch with your changes).
   
   c. GitHub displays the changes you have made between the two branches. Review them to ensure everything looks good.
   
   d. Click **Create pull request** and then click **Merge** to merge your changes from the working branch to the main branch. 

5. Wait for a few minutes for the content to be published. You can view your live website at `http(s)://<yourusername>.github.io/<yourusername>`.
