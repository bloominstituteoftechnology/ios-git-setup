# Installation Instructions

## 0. Download this repo from GitHub

1. Go to https://github.com/LambdaSchool/ios-git-setup.
2. Click **Clone or Download**.
3. Choose **Download ZIP**.
4. Open the resulting folder (`ios-git-setup`), and leave it to the side.

## 1. Download Textmate

1. Go to https://macromates.com/, and click `Download`.
2. Drag the app to your `/Applications` folder.
3. Open **Textmate**.
4. Go to the **Main Menu**, and choose **Textmate** > **Preferences…**.
5. Go to the **Terminal** tab.
6. Click **Install**.

This will allow you to use **Textmate** to edit git commits, and use other interactive features without needing to learn the ins and outs of `vi`/`vim`.

To make sure it works, do the following:
1. Open **Terminal**.
2. Type `mate .` at the command prompt.

A Textmate window should open. You can close it without saving.

## 2. Prep your `gitconfig` file

1. Open the provided `gitconfig` file with **Textmate** (or any other text editor).
2. Change `<Your Name Here>` on line 2 to be your name:
    - From: 	`name = <Your Name Here>`
    - To:	`name = Dimitri Bouniol`
3. Change `<youremailhere>` on line 3 to be your email (the one you use with GitHub):
    - From: 	`email = <youremailhere>`
    - To:	`email = dimitri.bouniol@lambda.com`
    
**Note:** If you've been using git for a while now, you can reference what you've been using by typing `less ~/.gitconfig` in **Terminal**

4. Change `<shortusername>` on line 10 to be your computer's short username:
    - From: 	`hooksPath = /Users/<shortusername>/.githooks`
    - To:	`hooksPath = /Users/dimitribouniollambda/.githooks`
    
**Note:** If you're not sure what your short username is, typing `echo ~` in **Terminal**, and use whatever is printed out there as the value for hooksPath, adding `/.githooks` to the end of that:

- `$  echo ~`
- `=> /Users/dimitribouniollambda`
- So you should use `/Users/dimitribouniollambda` + `/.githooks` => `/Users/dimitribouniollambda/.githooks`
    
5. Save the file.

## 3. Enable hidden files in Finder

1. Navigate to the `ios-git-setup` folder in the **Finder**.
2. Press **Shift-Command-Period** to enable/disable hidden files in the **Finder**.

## 4. Rename your new git configuration files

1. Rename `gitattributes` to `.gitattributes` (with a `.`). If you can't do this, see the above step for toggling hidden files and try again.
2. Rename `gitconfig` to `.gitconfig` (with a `.`).
3. Rename `githooks` to `.githooks` (with a `.`).
4. Rename `gitignore` to `.gitignore` (with a `.`).

They should all be slightly greyed out now.

## 5. Remove old git configuration files

1. In a new window, navigate to your home directory:
    - Go to the **Main Menu**, and choose **File** > **New Finder Window…** to open a new window.
    - Go to the **Main Menu**, and choose **Go** > **Home…** to go to your home directory.
2. Locate any of the following files: (you will need to have hidden files visible — see [#3-enable-hidden-files-in-finder](3. Enable hidden files in Finder))
    - `.gitattributes`
    - `.gitconfig`
    - `.githooks`
    - `.gitignore`
3. Rename them to not start with a `.`.

These files will not not be shaded out. You can now delete them if you'd like.

**Note:** If you also have a `.git` folder in your home directory, this was probably a mistake, and should probably be deleted. Reach out to your instructor for assistance.

## 6. Drag in the new git configuration files

1. Find the window for the `ios-git-setup` folder in the **Finder**.
2. Drag the following files (and one folder) from this window to the window with your **Home** directory:
    - `.gitattributes`
    - `.gitconfig`
    - `.githooks`
    - `.gitignore`

Congratulations! `git` should now be properly set up on your system 🎉