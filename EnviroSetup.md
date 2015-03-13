# Introduction #

This page will help you get your environment setup to:
1) Download the source code
2) Make changes
3) Commit changes
4) Push changes to repository

You must already have Visual Studio installed, I got my 2010 version for free through dreamspark.

Time to setup < 30 min.


# Details #

## XNA ##
First things first, we need to install the language libraries that we are using! Go ahead and go to dreamspark and download XNA4.0. Once it is done downloading go ahead and install it, should not take too long.

## GIT ##
Now you should go ahead and download git, as this is what we are using for this repository. Here is the version that I installed: [GIT](http://code.google.com/p/msysgit/downloads/detail?name=Git-1.7.9-preview20120201.exe&can=2&q=). Just follow the prompts to get a generic install.

## GIT Extensions ##
Next up you need to install [GIT Extensions](http://gitextensions.googlecode.com/files/GitExtensions228SetupComplete.msi). Follow the promps to install the basic setup.

## Visual Studio ##
Now you need to open up Visual Studio. At the top you should see a menu called "**Tools**". Open this and select "**Extension Manager**". Now on the left click "**Online Gallery**" then in the search bar on the top right type "git". Hit enter. You should now see several results, the one we want is called "**Git Source Control Provider**". Double click to install.

Once the extension has fully installed, you might be prompted to restart. Do so. Afterwards, go ahead and open up "**Tools**->**Options**". Browse to the "Source Control" submenu, and select the one for git. Once  this is open you should see several fields for a Path to git, git extensions, etc.

Go ahead and click the "Browse ..." button for Git Bash. Navigate to where you installed git in the steps above. The file you are looking for is called "**sh.exe**". For me this was:

` C:\Program Files (x86)\Git\bin\sh.exe `

No click the "Browse ..." button for Git Extensions. Navigate to where you installed git extensions from above. For me this was:

` C:\Program Files (x86)\GitExtensions\GitExtensions.exe `

Congrats! Your visual studio is now setup... for the most part.

## Downloading a Clone ##
Now we need to download a copy of the repository for you to use. Go ahead and navigate to the Source tab above: [Source](https://vandolis@code.google.com/p/ucsd-sweatervest-game/source/checkout)

Follow these instructions to download a copy of the repository onto your computer. Now for a bit of ease-of-use tweaks.

On that page you should have seen something about "**.netrc**". On windows installs this is actually called "_**netrc**". We want to add this file in our home directory... which windows doesn't know about. First we need to make a home directory PATH._

Open a command prompt. Now type: `setx HOME %USERPROFILE%`

This will create a new PATH called HOME. Now you just need to add your _netrc file to this directory (c:\users\YOU\)_

Edit this file and insert: `machine code.google.com login <YOUR LOGIN> password <YOUR PASSWORD>`
Where your login is your email account tied to this project, and your password is found in your google profile.

Save it and you are good to go!

From now on however, do not reference the repository like: `https://vandolis@code.google.com/p/ucsd-sweatervest-game/`
instead use: `https://vandolis@code.google.com/p/ucsd-sweatervest-game/`
else you will get errors.