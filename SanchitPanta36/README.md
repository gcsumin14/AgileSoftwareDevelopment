# Lab Submission Guide

This guide explains how to submit your lab PDF to the GitHub repository using either:

- **Method 1:** GitHub Web Interface (No Git installation required)
- **Method 2:** Terminal (Git CLI)

---

# Method 1: Using GitHub Website

## Step 1: Fork the Repository

1. Open the original GitHub repository.
2. Click the **Fork** button in the top-right corner.
3. GitHub will create a copy of the repository under your GitHub account.

---

## Step 2: Open Your Fork

1. Go to your GitHub profile.
2. Open the forked repository.

---

## Step 3: Create Your Folder

GitHub does not allow empty folders, so create a folder by creating a file inside it.

1. Click **Add file** → **Create new file**.
2. In the filename box, enter:

```
YourNameRoll/README.md
```

Example:

```
JohnDoe_45/README.md
```

3. Add the following content:

```
My Lab Work Folder
```

4. Click **Commit changes**.

---

## Step 4: Upload Your PDF

1. Open the folder you just created.
2. Click **Add file** → **Upload files**.
3. Drag and drop your PDF.

Example:

```
Lab1_Agile.pdf
```

Your repository structure should look like:

```
RepositoryName/
└── YourNameRoll/
    ├── README.md
    └── Lab1_Agile.pdf
```

4. Click **Commit changes**.

---

## Step 5: Create a Pull Request

1. Open your fork.
2. Click **Contribute** → **Open pull request**.
3. Review your changes.
4. Click **Create pull request**.
5. Submit the pull request.

The repository owner will review and merge your submission.

---

# Method 2: Using Terminal (Git)

## Step 1: Fork the Repository

1. Open the original repository.
2. Click **Fork**.
3. Wait until GitHub creates your copy.

---

## Step 2: Clone Your Fork

Replace the username and repository name with your own.

```bash
git clone https://github.com/YourUsername/RepositoryName.git
```

Move into the project folder.

```bash
cd RepositoryName
```

---

## Step 3: Create Your Folder

Create a folder using your name and roll number.

```bash
mkdir YourNameRoll
```

Git does not track empty folders, so create a README file.

```bash
echo "My Lab Work Folder" > YourNameRoll/README.md
```

---

## Step 4: Copy Your PDF

Copy your PDF into the folder.

Example:

```bash
cp ~/Downloads/Lab1_Agile.pdf YourNameRoll/
```

Your directory should look like:

```
RepositoryName/
└── YourNameRoll/
    ├── README.md
    └── Lab1_Agile.pdf
```

---

## Step 5: Verify the Changes

Check the repository status.

```bash
git status
```

You should see something similar to:

```
new file: YourNameRoll/README.md
new file: YourNameRoll/Lab1_Agile.pdf
```

---

## Step 6: Add the Files

Stage all changes.

```bash
git add .
```

---

## Step 7: Commit the Changes

Create a commit.

```bash
git commit -m "Add Lab 1 submission"
```

---

## Step 8: Push to GitHub

Push your changes to your fork.

```bash
git push origin main
```

If your default branch is `master`, use:

```bash
git push origin master
```

---

## Step 9: Create a Pull Request

1. Open your fork on GitHub.
2. Click **Compare & pull request**.
3. Review the changes.
4. Click **Create pull request**.
5. Submit the pull request.

The repository owner will review and merge your submission.

---

# Repository Structure

Your repository should look similar to:

```
RepositoryName/
│
├── Student1_01/
│   ├── README.md
│   └── Lab1_Agile.pdf
│
├── Student2_02/
│   ├── README.md
│   └── Lab1_Agile.pdf
│
└── Student3_03/
    ├── README.md
    └── Lab1_Agile.pdf
```

---

# Important Notes

- Fork the repository before making changes.
- Always work in **your fork**, not the original repository.
- GitHub does not allow empty folders.
- Every folder should contain a `README.md` file.
- Keep your PDF inside your own folder.
- Verify changes with `git status` before committing.
- Push your changes before creating a Pull Request.
- If requested, update your existing Pull Request instead of creating a new one.

---

# Common Git Commands

```bash
git clone <repository-url>
cd RepositoryName
mkdir YourNameRoll
echo "My Lab Work Folder" > YourNameRoll/README.md
cp ~/Downloads/Lab1_Agile.pdf YourNameRoll/
git status
git add .
git commit -m "Add Lab 1 submission"
git push origin main
```

---

# Submission Checklist

- ✅ Forked the repository
- ✅ Cloned your fork (Terminal method only)
- ✅ Created your folder
- ✅ Added `README.md`
- ✅ Uploaded the lab PDF
- ✅ Committed the changes
- ✅ Pushed to GitHub
- ✅ Created a Pull Request

---

# Done!

Your lab has now been successfully submitted through GitHub. Once your Pull Request is reviewed and merged, your submission will become part of the original repository.
