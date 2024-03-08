# How to Host your Resume on GitHub Pages

## Purpose
This guide outlines how you can host your resume as a static website (built for you) for free, using GitHub Pages. These steps **can be done by anyone**, even those without any prior knowledge of website hosting or experience in web design/development!

We will be using Markdown, a Markdown Editor (VS Code is our choice), and GitHub Pages to create our static resume website.

## Table of Contents
- **[Prequisites](#prerequisites)**
- **[Instructions](#instructions)**
- **[More Resources](#more-resources)**
- **[Authors & Acknowledgements](#authors--acknowledgements)**


## Prerequisites
Before we begin, the following things are required; there are links to help you complete these in the **[More Resources](#more-resources)** section.
1. **Understanding of Markdown (`.md`) files.**
    - Since our GitHub Pages' use markdown files to display its content, you need to know how to write a Markdown file.
2. **GitHub Account**
    - You'll need a GitHub account to be able to use the GitHub Page hosting feature.
3. **A program to edit/create Markdown .md files.**
    - In order to create Markdown files, you'll need an editor. I suggest using **[VS Code](https://code.visualstudio.com/download)**.
3. **An existing Resume**
    - Have your resume ready to be converted into a Markdown file.

## Instructions

### 1. Create a Resume Markdown File

This will be the Markdown file which displays on your GitHub Page. We will name it `index.md` because web browsers look for the *Index* as the starting page for websites; it works the same way for GitHub Pages.

1. Open your editor of choice, and create a file named `index.md`.
2. Write out your resume in Markdown form. 
    - Check out Markdown resources in **[More Resources](#more-resources)** to see the powerful formatting options Markdown has, and to see an example of resume already in `.md` format.
    - **Tip:** Press CTRL + SHIFT + V to see a live preview of the final Markdown product in VS Code.

![Step1](https://github.com/dev-jalapeno/dev-jalapeno.github.io/blob/main/assets/step1.gif)

> In Andrew Etter's book, Modern Technical Writing, he describes Markdown as a lightweight markup language (derived from XML). It offers a small and simple toolset that heavilty emphasizes readability and formatting without sacrificing a documents professional demeaner. In contrast, XML also has these results, without any of the approachability advantages, due to it's complex syntax.

### 2. Login to GitHub
Login to your GitHub account, and go to the [homepage](https://github.com/dashboard).

> Etter makes a point to make a version control systems, like Distributed Version Control Systems (DVCS), part of your project workflow. It allows multiple users to collaborate on a project, with tools for conflicting files, and an in-depth history management system. He also mentions that these DVCS, such as Git, offer advatanges for a wide range of users; developers, technical writers, etc. Some of these benefits include the ability to work offline, file synchronization among teams and branches (environments), backup restoration (rollback) and more. For technical writers, this toolset allows them to keep documents up to date, see previous versions of said documents, and easily make additions or changes.

### 3. Create your Repository
Now we need to create a repository; a project that acts like an online folder, which will contain our files needed to host the webpage.

1. Click **[+New]** button to create a new repository. 
2. Under **Repository name**, enter `username.github.io`, where `username` is your <u>exact</u> GitHub username. Everything else is purely optional, and should be left untouched.
3. Click **[Create repository]**.

![Step3](https://github.com/dev-jalapeno/dev-jalapeno.github.io/blob/main/assets/step3.gif)

### 4. Upload your Resume `(index.md)`
Next, we will upload the resume file we created. 

**IMPORTANT!** Ensure your resume file is named `index.md`, or else your resume won't display properly.

Click <u>**uploading an existing file**</u> and drag your file into the window. If you can't find this button, go to `https://github.com/username/username.github.io/upload`, once again replacing `username` with your username.

![Step4](https://github.com/dev-jalapeno/dev-jalapeno.github.io/blob/main/assets/step4.gif)

### 5. Setup GitHub Pages Intergration
Finally, we need to just turn on Pages under our repository settings. Currently, it's disabled because we haven't selected a `branch` for it look in. 

A branch one of environments of the repository, which are used to having multiple versions of the files at once. For our purposes, we will have only 1, which was created for us already.

1. Go to **Settings** at the top of your repository.
2. Select the **Pages** category on the left.
3. Under the **Branch** section, select `main` or `master`; only one will exist for you.

![Step5](https://github.com/dev-jalapeno/dev-jalapeno.github.io/blob/main/assets/step5.gif)

> Andrew makes note of the strengths given by using a Static website. Normally, a website is complex beast; it is run using Content Management Systems, like Wordpress, on a server somewhere; or, it is run locally, where your computer still needs to run HTML/CSS and web-browser tasks to display it. Conversely, static webpages are built before-hand, and are usually written in simpler languages, like Markdown, making them approachable to nearly everyone. Thus, they are fast, losing the complex background processes, and can be hosted on various platforms. Finally, they are naturally less vulnerable to security flaws, since they lack the complex features that are commonly exploited.

### 6. Visit your new Website!
Your resume is now hosted using GitHub Pages. You can visit it at `https://username.github.io`.

Congradualations, you just hosted your resume online!

### 7. (Optional) Configure & Customize (Jekyll)
GitHub provides us a Markdown template by default. However, you can customize it using **themes**. This is powered by Jekyll, the static site generator that is creating our webpage.

For our purposes, we will be using GitHub Pages' **Remote Theme** feature, which allows us to use Jekyll themes created by other GitHub users with a simple `_config` file.

Take a look at **[this list](https://github.com/topics/jekyll-theme)** of themes or find your own online. Regardless, you'll need to scroll down and read the `README.md` to make sure it supports the **Remote Theme** feature.

I recommend the **[Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll)** theme by daattali.

1. Create a new file called `_config.yml` in your editor. 
    - Since this is a `YAML` filetype, not a Markdown one, you will need an editor that supports this. VS Code does support it.
2. Add `remote_theme: daattali/beautiful-jekyll`.
    - If you found another theme on GitHub replace the end part with `username/theme-name`. These come from the end of the URL from the theme's repository page.
3. Save and upload this file to your repository, as you did in **Step 4**.

![Step7](https://github.com/dev-jalapeno/dev-jalapeno.github.io/blob/main/assets/step7.gif)

> Etter states Jekyll is the most popular static website generator, especially for the purposes of documentation; it's flexible, adaptable, and lightweight. Its toolset includes features that elevate documentation, such as nested navigation menus, and easily-accessable configuration through it's global and per-document files, in _config.yml and the header of the file respectively.

## More Resources
### Markdown
- **[Quickstart Guide](https://www.markdowntutorial.com)**
- **[Cheatsheet for formatting](https://commonmark.org/help/)**
- **[Full Markdown breakdown](https://www.markdownguide.org/getting-started/)**
### GitHub
- **[Create a GitHub Account](https://github.com/signup)**
- **[GitHub Pages official documentation](https://docs.github.com/en/pages)**
### VS Code
- **[Download link](https://code.visualstudio.com/download)**
- **["What is VSCode?"](https://code.visualstudio.com/)**
### Jekyll
- **[List of themes](https://github.com/topics/jekyll-theme)** 
- **[Beautiful Jekyll theme](https://github.com/daattali/beautiful-jekyll)**
- **[GitHub Pages' Jekyll Integration](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)**

## Authors & Acknowledgements
- **Alejandro Labra** - README and Hosting Guide.
- **Maria Luisa** - Peer Reviewed `README.md`.
- **daattali** - [Beautiful Jekyll theme.](https://github.com/daattali/beautiful-jekyll)

## Frequently Asked Questions (FAQs)

### *Why is Markdown better than a word processor?*
Markdown is naturally lightweight; its toolset is small, but powerful. It's also free, as it's a filetype that is supported by a number of free applications. In contrast, word processors are used best for fixed, formatted documents. Thus, they require strict exporting options, such as PDF formatting, and rarely have support for seamless content sharing.

Furthermore, it focuses on the content, layout and accessability of the document over appearance. Thus, it is naturally professional when the toolset is used appropriately.

Additionally, Markdown has become the default langauge for many technical writing and developer-focused software, such as GitHub, allowing for seamless integration and viewing of `.md` (Markdown) files.

### *Why is my resume not showing up?*
The most common reasons for your resume not displaying on your webpage are listed here.
- Your resume file may not be named `index.md`. Rename it and reupload it, making sure the `.md` part is included in the name; it is the actual filetype.
- You may have not named your repository the exact same name as your GitHub username, appended by `.github.io`. It should be `username.gihub.io`, where `username` is replaced by your GitHub username.
- You might have forgotten to select the `branch` in your repository's settings. Retry **Step 5.**
- If the above points are solved and you are still having issues, the GitHub Pages' Jekyll building may have failed. You will need to look into the build logs to request a rebuild. Refer to the GitHub Pages' documentation **[here](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-jekyll-build-errors-for-github-pages-sites)**.
