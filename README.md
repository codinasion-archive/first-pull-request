# First Pull Request

This project aims to help/guide beginners to make their first pull request.

---

## Ways to create a Pull Request

### Using Command Line

If you don't have git on your machine, [install it](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

#### 1. Fork this repository

Fork this repository by clicking on the fork button on the top of this page. This will create a copy of this repository in your account.

#### 2. Clone the repository

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the copy to clipboard icon.

Open a terminal and run the following git command :

```bash
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

For example :

```bash
git clone https://github.com/<your_username>/first-pull-request.git
```

where `<your_username>` is your GitHub username. Here you're copying the contents of the `first-pull-request` repository on GitHub to your computer.

#### 3. Create a branch

Change to the repository directory on your computer (if you are not already there) :

```bash
cd first-contributions
```

Now create a branch using the git checkout command :

```bash
git checkout -b your-new-branch-name
```

For example :

```bash
git checkout -b add-harshraj8843
```

(The name of the branch does not need to have the word add in it, but it's a reasonable thing to include because the purpose of this branch is to add your name to a folder.)

#### 4. Make necessary changes and commit those changes

Now create a file `<your_username>.json` inside `contributors` folder.

Add these lines inside `<your_username>.json`

```json
{
  "name": "<your_name>"
}
```

where `<your_username>` is your GitHub username and `<your_name>` is your name.

For example :

`harshraj8843.json` with content

```json
{
  "name": "Harsh Raj"
}
```

Now, save the file.

If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add command` :

```bash
git add <your_username>.json
```

Now commit those changes using the `git commit` command :

```bash
git commit -m "add <your_username>"
```

replacing `<your_username>` with your Github username.

#### 5. Push changes to GitHub

Push your changes using the command git push:

```bash
git push origin <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

#### 6. Submit your changes for review

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

Now submit the pull request.

Soon your pull request will be reviewed and merged into the master branch of this project. You will get a notification email once the changes have been merged.
