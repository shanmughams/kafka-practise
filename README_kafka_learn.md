
# kafka-learn

This repository is intended for learning and experimenting with Kafka. Follow the instructions below to set up a local Git repository and connect it to GitHub on Windows 11.

## Prerequisites

- Ensure Git is installed on your Windows 11 machine. Download it from [git-scm.com](https://git-scm.com/).

## Steps to Set Up and Connect the Repository

### 1. Configure Git

1. Open **Git Bash**.
2. Set up your Git username and email:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your_email@example.com"

   git config --global user.name "Shanmugham S"
   git config --global user.email "shanmughams@gmail.com"
   ```
3. Verify your Git configuration:
   ```bash
   git config --list
   ```

### 2. Create a Local Repository

1. Open **Git Bash** in the directory where you want to create your project (e.g., `Documents`).
2. Create a new directory for the project and navigate into it:
   ```bash
   mkdir kafka-learn
   cd kafka-learn
   ```
3. Initialize a new Git repository:
   ```bash
   git init
   ```

### 3. Create a New Repository on GitHub

1. Go to [GitHub](https://github.com/).
2. Click on **New** under the "Repositories" section.
3. Name the repository **kafka-learn** (to match the local repository name).
4. Set your preferred visibility (Public or Private).
5. Click **Create repository**.

### 4. Link the Local Repository to GitHub

1. In **Git Bash**, add the GitHub repository as a remote. Replace `your_github_username` with your GitHub username:
   ```bash
   git remote add origin https://github.com/shanmughams/kafka-learn.git
   ```
2. Verify the remote:
   ```bash
   git remote -v
   ```

### 5. Optional: Set Up SSH for Authentication

1. Generate an SSH key (if not already set up):
   ```bash
   ssh-keygen -t ed25519 -C "your_email@example.com"
   ```
   - Press `Enter` to accept the default location.
   - Optionally, set a passphrase.

2. Copy the SSH key to your clipboard:
   ```bash
   cat ~/.ssh/id_ed25519.pub
   ```

3. Add the SSH key to GitHub:
   - Go to **GitHub** -> **Settings** -> **SSH and GPG keys** -> **New SSH key**.
   - Paste the key and save it.

4. Test the SSH connection:
   ```bash
   ssh -T git@github.com
   ```

5. Switch the remote URL to SSH:
   ```bash
   git remote set-url origin git@github.com:shanmughams/kafka-learn.git
   ```

### 6. Add and Push Initial Commit

1. Create a `README.md` or another initial file:
   ```bash
   echo "# kafka-learn" > README.md
   ```

2. Add and commit the file:
   ```bash
   git add .
   git commit -m "Initial commit"
   ```

3. Push the commit to GitHub:
   ```bash
   git push -u origin main
   ```

## Verification

Your repository should now be connected to GitHub. Any further changes you commit and push will appear in your GitHub repository.

---

Happy coding!
