# How to Host a Resume on Github Pages

![An Example of the final resume hosted](/images/1_example_resume.gif)

A beginner's guide to host a markdown resume with a theme in the GitHub Pages.

## Prerequisites

Before we start the project make sure to have all of the following:

- **A Resume Formatted in Markdown**: if you already have a resume in PDF or word document checkout the [convertors listed](#convert-your-resume-to-markdown).
  - To make the process more smoothly, checkout the [index.md](/index.md) and try to follow that format with your resume. Its inspired by [this format](https://github.com/elipapa/markdown-cv/blob/master/index.md?plain=1).
- **Git**: make sure you have git installed in your computer. If you are unsure, you can download it [here](#git).
- **GitHub Account**: This is where your resume is going to be hosted.
  - If you need an account go to [GitHub SignUp](https://github.com/signup).
  - If you are new to GitHub checkout the [GitHub Resources](#github) for a quick start
- **Visual Studio Code**: This where you can edit your resume and use Git and GitHub seamlessly. You can download it [here](#visual-studio-code-vs-code).

## Instructions

Now that you have all the prerequisites, go to your browser and login to your github account.

### Making a Repository (Repo)

In your browser:

1. Go to [github.com](https://github.com/).
2. On your left panel click on **Create Repository**.
3. Create a repository with name in this format: `YourGitHubUSername.github.io`.
   - In the example below, my username is: _BarbTutorial_, so the name of my repository is going to be `BarbTutorial.github.io`.
4. Click on **Create a repository**.

You should see a page with a quick start available and a code to copy:

![Empty repository](/images/1_example_resume.gif)

#### Cloning your Repo to Visual Studio

> Before starting, make sure you have [Git]((https://git-scm.com/download/win)) and [Visual Studio Code](https://code.visualstudio.com/download) downloaded.
> As well as [connecting your GitHub account to Visual Studio Code](https://code.visualstudio.com/docs/sourcecontrol/github)

In Visual Studio Code

1. Open a new window
2. On the left nav bar, select the **Explorer**
3. On the left menu, Click on **Clone Repository**
4. On the top bar, Click on **Clone From GitHub**
5. Click on the one that says `YourGitHubName/YourGitHubName.github.io`
   - Following the example below, the repo is called `BarbTutorial/BarbTutorial.github.io`
6. Select the a place where you are going to store your copy of the repo
   - I recommend having a dedicated folder called **GitHub Projects** under the **Local Disk C:** where I store all my cloned repos.

You should see:

> add gif

### Uploading your resume

Now that your repo is cloned lets setup your resume.

1. On the File Explorer, find the file with your resume and copy it.
2. Open VS Code, on the left Nav Bar, select **Open Editor**.
3. On the left Menu that opens, paste the resume you copied into the repo.
4. Change the name of your markdown resume to `index.md` by right clicking the file and then on the option **Rename...**
   > This step is very important since this is how you tell GitHub Pages knows which file to display.
5. Open your `index.md` file and add the following to the top of your resume:

    ```md
    ---
        layout: cv
        title: Your Name's CV
    ---
    ```

6. Change the `Your Name's CV` to your name or an appropriate title for your resume.

If done successfully, you should see `index.md` with your resume in it on your left bar:

> add gif

### Adding a Theme

Now that you have a resume uploaded, lets add a theme so that it looks like a resume when you host it.

1. Go to [https://github.com/elipapa/markdown-cv](https://github.com/elipapa/markdown-cv)
2. Select **Code > Download ZIP**.
3. Unzip The file.
4. Open the unzipped folder and copy to your repo the file: `_config.yml` and the folders `_layouts` and `media`.

If done successfully, you should see the following on your left bar:

- `_config.yml`
- `_layouts`
- `media`.

> add gif

### Committing your changes

1. On the left Nav Bar, click to **Source Control**
2. Under Changes, click on the plus symbol on **Changes** to stage your changes.
3. Add a descriptive commit message like: _Adding resume and theme_.
4. Click on **Commit**.
5. Click on **Synch Changes**.

If done successfully, you should see the changes made on visual studio code on the your GitHub Browser.

> add gif

> If you need more help with commits in Visual Studio Code here is a [Commit Guide](https://www.youtube.com/watch?v=E6ADS2k8oNQ)

### Host your resume on GitHub Pages

Now that you have a resume to display, go to your repo with the format **YourGitHubUSername/YourGitHubUSername.github.io**

1. On the top **Nav Bar**, Go to **Settings**.
2. On the **Side Bar**, Go to **Pages**.
3. Click Stuff.

In the end you should see:

> add gif

### View your resume

Now give GitHub Pages some time to build your resume.

You can check if your time is done by:

1. On the Nav Bar, go to Actions.
2. Check the top `pages build and deployment` have a checkmark.

To see your website go to **https://YourGitHubUSername.github.io**.

In the example is: [https://barbzcodez.github.io](https://barbzcodez.github.io)

> add gif

Congratulations! You have a resume hosted on the web :)

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
- [Commit Guide](https://www.youtube.com/watch?v=E6ADS2k8oNQ)

### Template

- [CV Them Template](https://github.com/elipapa/markdown-cv)

## Author

Barbara Guzman Romero

## Acknowledgments

- Eliseo Papa for the CV Them Template

### Proof-readers

- Ryan Mack
- Eric Chu
- Thomas McIntosh

## FAQs

### Why is Markdown better than word or PDF?

Markdown better than word or PDF because:

- Is easier to learn and use.
- Easy to read even when it is just plain text, so without the theme.
- Widely used in the industry.
- You can personalize it as much or as little as you want and have a clean product.

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

### Why does my Resume isn't formatted properly?

A possible reason your resume isn't formatted properly, is because you missed a step or aren't following the .css rules

This is one example of what you might be looking at:

![A Screenshot of the sample resume with some text showing incorrectly](/images/badlyFormatted.png)

The problem was that there cant be a space between the date and the title

Incorrect:

```md
`Sept 2019 - May 2024`

__Bachelor of Computer Science Major (Co-op)__ | University of Manitoba, Canada
```

Correct:

```md
`Sept 2019 - May 2024`
__Bachelor of Computer Science Major (Co-op)__ | University of Manitoba, Canada
```
