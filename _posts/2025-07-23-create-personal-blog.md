---
title: "Host a portfolio on GitHub Pages"
date: 2025-07-23
tags: 
- technical writing
- GitHub
---

📑

Technical writers often need to provide writing samples to showcase their skills. While keeping them in a local storage is an option, a cloud-based portfolio makes your work accessible to others at any time. GitHub Pages provides a streamlined method for hosting static websites directly from a GitHub repository. 

## Introduction to GitHub Pages

GitHub Pages is a hosting service that generates a static website from files stored in a GitHub repository. It is ideal solution for personal blogs, portfolios, and project experiences.  

When you push content to your repository, GitHub Pages automatically builds and generates the site. To turn files into a site, GitHub Pages uses Jekyll, a built-in site generator. Jekyll uses themes to define the website's layout and style and there are plenty of themes ready for use. You can choose one of the available themes to create a professional website without configuring from scratch. 

> **Note:** While advances users can use CSS to customize or create themes, this topic focuses on building a site using an existing Jekyll theme. 

## Create a site from a GitHub repository

This section describes how to create a static site from a GitHub repository by using an existing Jekyll theme. 

### To create a site using a Jekyll theme:

1. Log in to [GitHub](https://github.com/) or sign up if you don't have an account.

2. Go to the [public Jekyll themes](https://github.com/topics/jekyll-theme) page, browse the themes, and select one for your site.

3. Open the target theme's repository and click **Fork** at top right. 
   ![fork a theme]({{ "/assets/images/posts/fork-a-theme.png" | relative_url }})
   
   > **Tip:** Fork means copy. Forking a Jekyll theme repository creates a copy of the  repository alongside all the configurations to your GitHub account. You can then add your website content by adding files to the copied repository. This is the simplest way to start using a Jekyll theme.

4. On the **Create a new fork** page, set the following fields:
   
   - **Owner:** This is auto-filled with your GitHub username.   
   
   - **Repository name:** Rename the repositiory to `YOURUSERNAME.github.io`, where `YOURUSERNAME` must be your GitHub username.     
     
     > **Note:** It's important to use your GitHub username, so that GitHub Pages can recognize it and create a website for your repository.

5. Click **Create fork** to copy the theme's repository to your GitHub account.

6. Open the copied repository on your GitHub account, click **Settings** at the top and then select **Pages** in the left pane.
   ![set pages]({{ "/assets/images/posts/set-pages.png" | relative_url }})

7. In the **Build and deployment** area, set the following fields:   
   
   - **Source:** Select **Deploy from a branch.**
   - **Branch:** Select **`main`** or **`master`**. 

8. Click **Save** to enable GitHub Pages for your repository. 
   When you add content files and commit your changes, GitHub Pages automatically generates and publishes the site. 

## Add content to your site

After creating and setting up the GitHub Pages site, you can now add content to it.

### To add content to your site:

1. Open your website repository and create a branch for it. 
   
   > **Tip:** A branch is an isolated working copy of your repository. We recommend that you make and test changes in a branch and then merge them into the main branch using a pull request.<br>
   
   <ol type="a">
   <li>At the top left, locate the branch selector dropdown (it usually displays <b><code>main</code></b> or <b><code>master</code></b>).</li>
   <li>Click the dropdown and then in the field that appears, type the name of your new branch, for example, <code>my-pages</code>.</li>
   </ol>

2. Select the new branch and then open the `README.md` file. The `README.md` file contains instructions on how to configure settings and manage content for the site. 

3. Follow the instructions in the `README.md` file to make the necessary site configurations and add content files, and then click **Commit changes** to save your changes.   
   
   > **Tip:** In order for the Jekyll theme to process the content files and turn them into a functional site, you must use the specified format for the content files and place the content files under the designated folder. For details about the configuration, follow the instructions in the `README.md` file.

4. After you have added content files for your website, review the files in the branch to make sure everything works fine, and then merge the changes to the main branch.
   
   <ol type="a">
   <li>Click <b>Pull requests</b> at the top.</li>
   <li>Under <b>Comparing changes</b>, select the <b>base branch</b> (usually <code>main</code> or <code>master</code>) and the <b>compare branch</b> (the branch with your changes).</li>
   <li>GitHub displays the changes you have made between the two branches. Review the changes to make sure everything looks good.</li>
   <li>Click <b>Create pull request</b> and then click <b>Merge</b> to merge your changes from the working branch to the main branch.</li>
   </ol>

5. Wait for a few minutes for the content to be published. You can view your live website at `http(s)://<yourusername>.github.io/<yourusername>`.
