---
title: "Create a personal website"
date: 2025-07-23
tags: 
- technical writing
- GitHub
---

📑

Technical writers are often asked to provide writing samples to showcase their skills. Instead of storing them locally, creating a personal site for your portfolio makes it accessible from anywhere, at any time. One easy way to create a personal website is to create a GitHub Pages site from a GitHub repository. 

## Introduction to GitHub Pages

GitHub Pages is a GitHub feature that can create a static website directly from a repository. It works by connecting a GitHub repository to a website. You add content files to a GitHub repository and GitHub Pages automatically builds and publishes a website from these files. GitHub Pages are ideal for hosting static websites for personal blogs, portfolios, or resumes.<br>

To generate a site from files in a GitHub repository, a static site generator is needed. Jekyll is the built-in site generator for GitHub Pages. There are a vast number of Jekyll themes available for use. These Jekyll themes define the layouts and styles for a website and include configurations that are required to generate a site from GitHub repository files. Using an existing Jekyll theme lets you quickly create a site and avoids the need to configure everything from scratch. <br>

Users with knowledge in css can also customize an existing Jekyll theme to change the website layout and style, or even create a Jekyll theme to add more style to the website.  

This topic provides instructios on how to build a static site using an existing Jekyll theme. Customizing a Jekyll theme or creating a Jekyll theme is not covered in this topic. 

## Create a static site from GitHub repository

This section describes how to create a static site from a GitHub repository by using a Jekyll theme. A Jekyll theme defines the layout and style of a website. Using a Jekyll theme lets you build a site quickly and easily. 

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
