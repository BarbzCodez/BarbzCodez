# Hosting a Resume on GitHub Pages

## Purpose

According to Andrew Etter in [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) we want to "make content beautiful, discoverable and searchable." This guide will help you achieve Etter's goal by hosting a themed markdown resume using GitHub Pages.

![An Example of the final resume hosted](/images/1_example_resume.gif)

---

## Etter's Principles

Before starting, I would like to to explain how Etter's principles reflect on this project. I will list them and explain:

- _Use a lightweight markup_: We want content that is readable without the need to export it. We will be achieving this by using Markdown to write your resume as it is very simple to learn and use.
- _Use distributed version control_: We want to one version of truth with a history of how we got there. we'll be achieving that by using GitHub, which is easy to start using and widely used.
- _Make static websites_: Etter likes static websites because they are simple and usually free to use. We are using GitHub Pages to host our static website because is integrated with GitHub.

---

## Prerequisites

Before we start the project make sure to have the following:

- **A Resume Formatted in Markdown**: This is the resume that is going to be shown.
  - If you already have a resume in PDF or word document checkout the [convertors listed](#convert-your-resume-to-markdown).
  - Start with the sample resume on [index.md](/index.md) as template.
  - For more information checkout the [template section](#template) on the resources.
- **Git**: This is where you can make changes locally and push them to GitHub.
  - You can download it [here](https://git-scm.com/download/win).
- **GitHub Account**: This is where your resume is going to be hosted.
  - If you need an account go to [GitHub SignUp](https://github.com/signup).
- **Visual Studio Code**: This where you can edit your resume and use both Git and GitHub seamlessly.
  - You can download it [here](#visual-studio-code-vs-code).

---

## Instructions

Now that you have everything, lets begin!

### Making a Repository

In your browser, login to your Github account.

1. Go to [github.com](https://github.com/).
2. On your left panel click on **Create Repository**.
3. Create a repository with name in this format: `YourGitHubUsername.github.io`.
   - In the example below, my username is: _BarbTutorial_, so my repository will be called `BarbTutorial.github.io`.
4. Checkmark the **Add a Readme** box.
5. Click on **Create a Repository**.

After, you will see your repository `YourGitHubUsername.github.io` with a readme.

![Empty repository](/images/2_create_repo.gif)

---

### Cloning your repository to Visual Studio Code (VS Code)

> Before starting, make sure you have [Git](https://git-scm.com/download/win) and [VS Code](https://code.visualstudio.com/download) downloaded.
> As well as [connecting your GitHub account to VS Code](https://code.visualstudio.com/docs/sourcecontrol/github)

Open a VS Code.

1. On the left nav bar, click on **Explorer**.
2. On the left menu, click on **Clone Repository**.
3. On the top bar, click on **Clone From GitHub**.
4. Click on the one named `YourGitHubName/YourGitHubName.github.io`.
   - In this example, the repository is called `BarbTutorial/BarbTutorial.github.io`.
5. Click on the folder where you are going to store a copy of the repository.
   - I recommend having a dedicated folder called **GitHub Projects** under **Local Disk C:** to store all your cloned repositories.
6. If you get a popup window, click on  **Open**.

By the end you should be able to see your repository in VS Code.

![Empty repository in VSCode](/images/3_cloning_repo_to_VSCode.gif)

---

### Uploading your Resume

Now let's add your resume.

1. Open **File Explorer**, find your markdown resume file and keep it to one side of the screen.
2. Open VS Code, on the left nav bar, have the **Open Editor** bar open.
3. Drag your resume from the **File Explorer** to the open editor in **VS Code**.
4. Change the name of your markdown resume to `index.md` by right clicking the file and then clicking on the option **Rename...**.
   > This step is very important since this is how you tell GitHub Pages which file to display.
5. Open your `index.md` file and add the following to the top of your resume:

    ```md
    ---
        layout: cv
        title: Your Name's CV
    ---
    ```

6. Change the `Your Name's CV` to your name.

If done successfully, you should see `index.md` with your resume in it on your left bar:

![your resume with named index](/images/4_uploading_your_resume.gif)

---

### Adding a Theme

Now that you've uploaded a resume, add a theme so that it looks like a resume on your website.

1. Go to [https://github.com/elipapa/markdown-cv](https://github.com/elipapa/markdown-cv)
2. Click on **Code > Download ZIP**.
3. Click on **Extract All** to unzip the files.
4. Open the extracted folder and drag the following files into your repository: `_config.yml` and the folders `_layouts` and `media`.
   > If you get a popup asking if you want to copy the media or folder, click  **Copy Folder** and it would be added to your side bar.

If done successfully, you should see the following on your Explorer:

- `_config.yml`
- `_layouts`
- `media`

![adding a theme to your repository](/images/5_adding_a_theme.gif)

---

### Committing your Changes

1. On the left Nav Bar, click on **Source Control**.
2. Under **Changes** you should see all the files you added, click on the plus symbol on **Changes** to stage your changes.
3. Add a descriptive commit message like: _Adding resume and theme_.
4. Click on **Commit**.
5. Click on **Sync Changes**.

If done successfully, then the changes made in VS Code should appear in the Repo which you can find in your browser using **YourGitHubUsername/YourGitHubUsername.github.io**.

![commit changes](/images/6_commit_your_changes.gif)

> If you need help with commits in VS Code here is a [Commit Guide](https://www.youtube.com/watch?v=E6ADS2k8oNQ)

---

### Hosting your Resume on GitHub Pages

Now that you have a resume to display, go to your repository with the format: **YourGitHubUsername/YourGitHubUsername.github.io**

1. On the top Nav Bar, Go to **Settings**.
2. On the Side Bar, Go to **Pages**.
3. Click on the **Visit Site**.

Congratulations! Your resume is now on the web :)

![see your resume on the web](/images/7_host_your_resume.gif)

Access your website at **https://YourGitHubUsername.github.io**. Replace YourGitHubUsername with your GitHub Username.

> In the example is: [https://barbtutorial.github.io/](https://barbtutorial.github.io/).

---

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
- [Connect GitHub to Visual Studio Code](https://code.visualstudio.com/docs/sourcecontrol/github)
- [Commit Guide](https://www.youtube.com/watch?v=E6ADS2k8oNQ)

### Template

- [Resume Theme Template](https://github.com/elipapa/markdown-cv)

## FAQs

### Why is Markdown better than word or PDF?

Markdown is better than word or PDF because:

- You can have one markdown file, apply a theme to make it into a website, document or even a presentation with one source of truth.
- Easy to read even as plain text, so no need to download anything to see the content.

### Why is my resume not showing up?

If your resume is not showing up I would recommend the following:

#### Check your settings

- If you just clicked on generate page; give it a minute. It takes Github Pages some time to build your page.
- Your Branch should say `main/root`

![successful settings](/images/FAQ1_settings.gif)

#### Check your actions

- Have all your checks passed? You can check this by going on actions and checking that all of the `pages build and deployment` have a checkmark.

![successful actions](images/FAQ2_actions.png)

#### Check your repository setup

- Make sure your resume information is in a file called `index.md`.
- Can you see the `index.md` on your git repository? If not, make sure to push all your changes to main.

![successful actions](images/FAQ3_repo.png)

## Author

Barbara Guzman Romero

## Acknowledgments

- [Eliseo Papa Resume Template](https://github.com/elipapa/markdown-cv).
- [Etter's Modern Technical Writing Book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS).

### Proof-readers

- Isabelle Anderson-Gregoire
- Thomas McIntosh
