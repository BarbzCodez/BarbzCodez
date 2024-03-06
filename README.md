# How to Host a Resume on Github Pages

![Insert gif here](/images/happy_dog.gif)

A simple guide to host a markdown resume in the GitHub Pages that looks like the gif!

## Prerequisites

Before we start the project make sure to have all of the following:

- **A Resume Formatted in Markdown**: if you already have a resume in PDF or word document checkout the [convertors listed](#convert-your-resume-to-markdown).
- **Git**: make sure you have git installed in your computer. You can check [here](#git).
- **GitHub Account**: This is where your resume is going to be hosted. If you need help check out the [GitHub Tutorial](#github).
- **Visual Studio Code**: This is a recommendation to edit your resume and use Git and GitHub seamlessly. You can download it [here](#visual-studio-code-vs-code)

## Instructions

Now that you have all the prerequisites, go to your browser and login to your github account.

### Making a Repository (Repo) for your Resume

In your browser:

1. Go to [github.com](https://github.com/)
2. On your left panel click on **Create Reository**
3. Create a repository with name in this format: `YourGitHubUSername.github.io`
   - In the example below, my username is: _BarbTutorial_, so the name of my repository si going to be `BarbTutorial.github.io`
4. Click on readme
5. Click on create a repository

You should see:

> add gif

#### Cloning your Repo to Visual Studio

> Before starting, make sure you have Git and [Visual Studio Code](https://code.visualstudio.com/download) downloaded. As well as [connecting your github account to Visual Studio Code](https://code.visualstudio.com/docs/sourcecontrol/github)

In visual studio

1. Open a new window
2. Click on **Explorer**
3. Click on **Clone Repository**
4. Click on **Clone From GitHub**
5. Select the a place where you are going to store your copy of the repo
   - I recommend having a dedicated folder called **GitHub Projects** under the **Local Disk C:** where I store all my cloned repos.
6. Click on the one that says `YourGitHubName/YourGitHubName.github.io`
   - In the example is `BarbTutorial/BarbTutorial.github.io`

You should see:

> add gif

### Uploading your resume

Now that your repo is cloned lets setup your resume.

1. On the file Explorer, find the file with your resume and copy it.
2. On Visual Studio Code, click the **Open Editor**.
3. Paste the resume you copied into the repo.
4. Change the name of your markdown resume to `index.md` by right clicking the file and then on the option **Rename...**
   > This step is very important since this is how you tell GitHub Pages knows which file to display.
5. Go to **Source Control**
6. Under Changes, click on the plus symbol on `index.md` to stage your changes
7. Add a commit message like: Adding resume
8. Click on Commit and then push

If done successfully, you should see `index.md` on your repo in GitHub on your browser.

> add gif

### Adding a Theme

Now that you have a resume uplaoded

1. On the file Explorer, find the file with your resume and copy it.
2. On Visual Studio Code, click the **Open Editor**.
3. Paste the resume you copied into the repo.
4. Change the name of your markdown resume to `index.md` by right clicking the file and then on the option **Rename...**
   > This step is very important since this is how you tell GitHub Pages knows which file to display.
5. Go to **Source Control**
6. Under Changes, click on the plus symbol on `index.md` to stage your changes
7. Add a commit message like: Adding resume
8. Click on Commit and then push

If done successfully, you should see `index.md` on your repo in GitHub on your browser.

> add gif

### Host your resume on GitHub Pages

Now that you have a resume to display, go to your repo with the format **YourGitHubUSername/YourGitHubUSername.github.io**

1. On the top **Nav Bar**, Go to **Settings**.
2. On the **Side Panel**, Go to **Pages**.
3. Click Stuff.

In the end you should see:

> add gif

### View your resume

Now give GitHub Pages some time to build your resume

You can check if your time is done by:

1. On the Nav Bar, go to Actions.
2. Check the top `pages build and deployment` have a checkmark.

If have 

Congratulations! You hav
e
## Resources

### Markdown

- [Markdown Tutorial](https://www.markdowntutorial.com)
- [Markdown CheatSheet](https://www.markdownguide.org/cheat-sheet/#basic-syntax)

#### Convert your Resume to Markdown

- [PDF to Markdown](https://pdf2md.morethan.io)
- [Word to Markdown](https://word2md.com)

### Git

- [Install Git on your computer](https://git-scm.com/download/win)

### GitHub

- [Create a GitHub Account](https://github.com/signup)
- [GitHub Tutorial](https://docs.github.com/en/get-started/start-your-journey/hello-world)

### Visual Studio Code (VS Code)

- [Download Visual Studio Code](https://code.visualstudio.com/download)
- [Connect Visual Studio Code to GitHub](https://code.visualstudio.com/docs/sourcecontrol/github)

### Advanced

- Jekill Tutorial
- Theme Examples
- Good Resume Tutorial

## Acknowledgments

### Templates

- The page for the theme
- The page for template

### Proof-readers

- Ryan Mack
- Eric Chu
- Thomas McIntosh

## FAQs

### Why is Markdown better than word or PDF?

Markdown better because:

- Is easier to learn and use.
- Easy to read even when it is not exported to a properly exported.
- Widely used in the industry.
- You can personalize it as much as you want

### Why is my resume not showing up?

If your resume is not showing up I would check the following:

#### Check your settings

- If you just clicked on generate page, it might take some minutes for the Github to build your page.
- Is your folder rooted in root

> add gif of what a successful page should look like

#### Check your actions

- Have all your checks passed? You can check this by going on actions and checking that all of the `pages build and deployment` have a checkmark

> add gif of what a successful page should look like

#### Check your repo setup

- Make sure your resume information is in a file called `index.md`.
- Can you see the `index.md` on your git repo? If not, make sure to push all your changes to main.

> add gif of what a successful page should look like

### Why does my `pages build and deployment` have a yellow dot?

If it has a yellow dot it means it needs more time. You can click on it to see the the progress of the build.
