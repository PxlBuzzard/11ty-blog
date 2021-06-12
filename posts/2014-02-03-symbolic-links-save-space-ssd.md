---
layout: layouts/post.njk
title: Using Symbolic Links to Save Space on Your SSD

date: 2014-02-03
published: false
tags: [Windows, advfoss, tutorial]
---

A common problem I run into after installing and using Windows on an SSD is that it quickly fills up. One great way to move files off the solid state is symbolic links. Symbolic links, or symlink, trick Windows into thinking that it is saving data to, say, `C:/Users/[username]/Documents`, when in reality the data is being saved to `D:/Documents`. Think of it like a folder shortcut, but at a deeper level.

#### Note

This operation works best on a relatively fresh install of Windows. I have used this method on Windows 7, 8, and 8.1. Your mileage may vary.

## Putting any folder onto another drive (GUI)

1. Use [Dirlinker](http://dirlinker.codeplex.com/).

![Dirlinker screenshot](http://res.cloudinary.com/danieljost/image/upload/v1391452418/Capture_uzhrdx.png)

##### What is that "If the link location exists" box asking about?

By creating a symbolic link, you are deleting the files from the original drive and storing them somewhere else. You can either choose to delete the files or copy them to their new home before making the link.

## Putting any folder onto another drive (command line)

1. Open the start menu and type `cmd` to open a command prompt. You may need Administrator permissions depending on your environment.

2. Modify `mklink /J "C:\The\Original\Location" "D:\New\Location"` to suit your needs. The \J means "directory junction," which is Microsoft's term for a symbolic folder link.

Example: `mklink /J "C:\Program Files (x86)\Steam" "D:\games"` creates a symlink for your Steam games and puts them onto a different drive.

## Moving the Users folder onto a different drive (hard mode)

You need to have a boot CD (or USB) for Windows for this tutorial.

1. Boot into the Windows boot CD, then load up the command prompt. For Windows 8, it looks like `Troubleshoot -> Advanced Options -> Command Prompt`.

2. Figure out which drive is which. **The drive letters are probably not the same as in your Windows environment.** You can access a drive by typing `C:`, and check its contents using `dir /w /p`. Write down which drive letters you will be using.

3. Type `robocopy /copyall /mir /xj C:\Users D:\Users`. Let's break that down:

	* `robocopy` copies files.
    * `/copyall` gets *all* the folders.
	* `/mir` copies the user permissions and other metadata.
    * `/xj` stops robocopy from following symbolic links.
    * `C:\Users` is your original Users folder (on your SSD or original drive).
    * `D:\Users` is where you want the Users folder to be stored from now on.

4. Type `rmdir /S /Q C:\Users`, replacing `C:\Users` with your original Users folder location.

5. Type `mklink /J "C:\Users" "D:\Users"`. `mklink \J` makes a symbolic link (or directory junction).

6. Exit the command prompt and boot back into Windows.

## Easily installing programs to SSD or HDD

My solution for choosing whether a program gets installed is simple: Create symbolic links named `nProgram Files` and `nProgram Files (x86)` that link to another hard drive. This way, in an installer you can put the `n` in the install location and have the program installed on your other drive.

![Install example](http://res.cloudinary.com/danieljost/image/upload/v1391454816/cap2_lhzitj.png)
