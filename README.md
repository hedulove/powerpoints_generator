

[![made-with-python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

## PowerPoint Generator: Your Gateway to Effortless Presentations 🚀

Dive into the ease of presentation creation with PowerPoint Generator, a smart web application crafted to automate 
PowerPoint presentations! 🌟 
This project is ripe for growth and eager for your contributions. Let's enhance its capability together! 😊

## Demo Highlights 🎬

## Table of Contents 📋

1. [Features](#features)
2. [Inner Structure of the Project](#inner-structure-of-the-project)
3. [How to Use](#how-to-use)
4. [How to Contribute](#how-to-contribute)

## Features 

* **🤖 AI-Driven Content Creation**: Utilize the power of GOOGLE GEMINI to generate slide content based on user's input.
* **😎 Intelligent Slide Generation**: The tool intelligently proposes titles and content for each slide.
* **🎨 Customizable Themes**: Choose color themes for your presentation, giving it a personalized touch.
* **🙂 User-Friendly Interface**: Clear instructions and an intuitive design make the PowerPoint generation process seamless and straightforward.

## Inner Structure of the project 

If you want to learn how to use the GPT API for creating PowerPoint presentations or understand how the project is 
organized, check out [CODE_STRUCTURE.md](docs/CODE_STRUCTURE.md). 🧐
In this document, I explain the code and the relationships between different parts of the code.

## How to use

If you want to try using this project, here is a step-by-step guide. 
Those who want to contribute to (which is welcome!), please check [How to Contribute](#how-to-contribute)

<details>
<summary>
Step 1: Star The Repo ⭐️
</summary>

Star the repo to start using this project 👍

![star repo](https://docs.github.com/assets/images/help/stars/starring-a-repository.png)

</details>

---

<details>
<summary>
Step 2: Clone It 🐑
</summary>

- **Using Git** 

Open your terminal and run the following command:

```bash
git clone https://github.com/account/project.git
```

- **Using Download ZIP**

1. Go to the GitHub page of the repository.
2. Click on the green **Code** button.
3. In the dropdown menu, select **Download ZIP**.

</details>

---
<details>
<summary>
Step 3: Create a Virtual Environment 📟
</summary>

On Windows 🪟
- Open your **Command Prompt** and navigate to your project's directory.
- Run the command line by line.
    ```bash
    python -m venv venv
    .\venv\Scripts\activate
    pip install -r requirements.txt
    ```
On macOS and Linux 🐧
- Open your **Terminal** and navigate to your project's directory.
- Run the command line by line.
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```
</details>

---

<details>
<summary>
Step 4: Setup API Keys 🔑
</summary>

⚠️ This step is very important to make the project work! 
please make sure if you set up everything correctly. 
Instruction ▶️ [Setup the Secret Key and Gemini Key](set-up-api-keys)

</details>

---

<details>

<summary>
Step 5: Run 🏃‍
</summary>

Navigate to `myapp` directory. Run `flaskapp.py`

```bash
python3 myapp/flaskapp.py
```

</details>

## How to contribute 

Thank you for considering how you can contribute to the project! ✨

<details>
<summary>
Step 1: Star The Repo ⭐️
</summary>

Star the repo to start your contribution ⭐️

![star repo](https://docs.github.com/assets/images/help/stars/starring-a-repository.png)

</details>

---

<details>
<summary>
Step 2: Fork it 🍴
</summary>

</details>

---

<details>
<summary>
Step 3: Clone it 🐑
</summary>

- **Method 1:** GitHub Desktop

> ⚠️ **NOTE:** If you're not familiar with Git, using **GitHub Desktop Application** is a better start. If you choose this method, make sure to download it before continuing reading.
>
> ❗❗ Access link to download [**here**](https://desktop.github.com).

- **Method 2:** Git

Clone the **forked repository**. Open terminal (command prompt) and type:

```bash
git clone https://github.com/<your-github-username>/PowerPoint-Generator-Python-Project.git
```

> This makes a local copy of the repository in your machine.
>
> ⚠️ **Replace \<your-github-username\>!**

</details>

---

<details>
<summary>
Step 4: Create your feature branch 🌴
</summary>

Always keep your local copy of the repository updated with the original repository.
Before making any changes and/or in an appropriate interval, follow the following steps:

- **Method 1:** GitHub Desktop

Learn more about how to create new branch [here](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/managing-branches#creating-a-branch) and how to fetch and pull origin from/to your local machine [here](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/keeping-your-local-repository-in-sync-with-github/syncing-your-branch).

Learn more about how to fetch and pull origin from/to your local machine using **GitHub Desktop** [here](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/keeping-your-local-repository-in-sync-with-github/syncing-your-branch).

- **Method 2:** Git

Run the following commands **_carefully_** to update your local repository.

```bash
# If you cloned a while ago, get the latest changes from upstream
git checkout main
git remote add upstream https://github.com/account/project.git
git pull upstream main

# Make a feature branch (Always check your current branch is up to date before creating a new branch from it to avoid merge conflicts)
git checkout -b <branch-name>

```

</details>

---
<details>
<summary>
Step 5: Pull Request 🖐️
</summary>

1. Open the GitHub website and find your forked repository.
2. On your fork's GitHub page, click 'New Pull Request'.
3. Ensure the base branch is the original repository's branch you want to merge into(main branch), 
and the compare branch is your feature branch.
4. Click 'Create Pull Request', add a title and a brief description of your changes.

Thank you for your contribution! 
I'll check your pull request. 😀

</details>

---

If you want to learn more about how to contribute, visit [CONTRIBUTING.md](docs/CONTRIBUTING.md).

## Setup the Secret Key and Gemini AI Key 

The application uses a secret key for session management and an Gemini key for the Gemini API.
These keys are defined as environment variables, and you can easily set them up using the provided .env.example file.

1. Locate the file named .env.example in the project directory.
2. Copy the contents of .env.example into a new file named .env.
3. Replace the placeholder values with your actual keys:
   
```
SECRET_KEY=your_secret_key
GEMINI_KEY=your_geminiai_key
PEXELS_API_KEY=your_pexels_key
```

Here's a brief description of each key and how to obtain them:

**SECRET_KEY**: 🔐This is used for web application security such as session management. You can create your own secure, random string for this.

**GEMINI_KEY**: 🤖This is required to access the GEMINI API. Although there's a limitation with the free version, it's sufficient for trying out this web application on your local machine. You can obtain this key by creating an account on the https://gemini.google.com.

**PEXELS_API_KEY**: 🏞️ This key is used for the free image search API provided by Pexels. It's very useful for adding creative images to your presentations. You can get this key by creating a free account on the https://www.pexels.com/api
After registering, the API key is automatically generated for you.


## Contributors ✨



<img src="https://github.com/otahina.png" width="50" height="50" alt="description">
<a href="https://github.com/otahina">Ota Hina</a>
<img src="https://github.com/gaganmanku96.png" width="50" height="50" alt="description">
<a href="https://github.com/gaganmanku96">Gagandeep Singh</a>


## License 📄

This project is licensed under the terms of the MIT license.




