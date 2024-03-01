# Practical Exercise: Deploying a Simple Application with GitHub Pages

This module provides a hands-on exercise for deploying a simple static website using GitHub Pages. By the end of this exercise, you will have deployed a basic HTML web page accessible on the internet.

## Prerequisites

- A GitHub account. If you don't have one, sign up at [https://github.com/](https://github.com/).
- Basic knowledge of HTML and Git.
- Git installed on your computer.

## Step 1: Create Your Simple Application

1. **Create a new directory** on your computer for your project. This can be done using the File Explorer (Windows) or Finder (Mac), or through the terminal/command prompt.

2. **Create a simple HTML file**. Inside your project directory, create a file named `index.html` and add the following HTML code:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>My Simple Application</title>
    </head>
    <body>
        <h1>Hello, GitHub Pages!</h1>
        <p>This is my first static site deployed using GitHub Pages.</p>
    </body>
    </html>
    ```

3. **Open your terminal or command prompt** and navigate to your project directory.

## Step 2: Initialize a Git Repository

1. Run `git init` to initialize a new Git repository in your project directory.

2. Add your file to the repository using `git add index.html`.

3. Commit your file to the repository with `git commit -m "Initial commit"`.

## Step 3: Create a Repository on GitHub

1. **Log in** to your GitHub account and go to the Repositories tab.

2. Click the **New** button to create a new repository.

3. **Name your repository**. It's a good practice to give it the same name as your local project directory.

4. **Do not initialize** the repository with a README, .gitignore, or license. Since your local repository already has content, initializing it on GitHub might complicate the process.

5. Click the **Create repository** button.

## Step 4: Push Your Application to GitHub

1. After creating your repository, GitHub will display a page with a quick setup URL. Copy the URL provided under "...or push an existing repository from the command line."

2. Go back to your terminal or command prompt, ensure you're still in your project directory, and run the following commands, replacing `<your-repository-URL>` with the URL you just copied:

    ```bash
    git remote add origin <your-repository-URL>
    git branch -M main
    git push -u origin main
    ```

## Step 5: Deploy with GitHub Pages

1. On GitHub, navigate to your repository.

2. Go to the **Settings** tab, then find the **Pages** section on the left sidebar.

3. In the **Source** section, select the `main` branch as your source. If you've created a `/docs` folder or have a different setup, select accordingly. Leave the folder as `(root)` if your `index.html` is in the root directory.

4. Click **Save**, and GitHub will automatically deploy your site.

5. GitHub Pages will provide a URL to access your site. It may take a few minutes for the site to become available.

Congratulations! You've successfully deployed a simple static website using GitHub Pages. Visit the provided URL to view your application live on the internet. This exercise demonstrates the deployment phase in the SDLC, showcasing how you can quickly and efficiently make a website accessible to users worldwide.