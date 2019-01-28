## Talk Notes

based on 5 Essential Ingredients for an Awesome Tech Talk by [David Neal](https://reverentgeek.com/5-essential-ingredients-for-an-awesome-tech-talk/)

## 1. Why did you choose this technology?
Problem that needed solving:
Needed to distrbute a simple command line app out to others.
At my work we had a task that I created a command line tool to automate for myself. I wanted to give this tool out to others so that they could use it too.
These users aren't developers so running command line apps isn't something they have a lot of experience with. Needed to make it simple. Folks have experience with chat and can follow a prompt that walks them through the process. But, getting it installed on everyone's machine and teaching them to work through a command line would be too much. I would need to provide instruction on how to install Node.js, and how to npm install the project dependencies, and then how to navigate their system via the command line to run the tool. That would get too complex for those without code / development experience.
I looked at Electron to make a simple app, but didn't need a complex UI. Using a command line interface that walks someone through two or three questions would be enough.
If I could take the script and package it up to give out that would be awesome.
Also, we have both macOS and Windows users in our group. So, the solution needs to be something that can be given out to all users regardless of their OS.
Then I came across PKG and how it can do exactly that.

Made by Zeit who make other interesting / cool OSS projects like Hyper & Next.js
Simple to use. Not much change is needed to the existing project / workflow to get it working
Can make easily distributable executable (fun to say :) ) that others can download and install just by placing in a folder on their system.



## 2. What does this technology do?
Describes itself as a "Single-Command Node.js Binary Complier."
Command line app that takes a Node.js project and packages it up to be run on its own. Node.js doesn't even need to be installed to use the project. Everything, including the necessary Node.js binaries are inlcuded in the final compiled project.

Can be run with a simple command to output a version for macOS, Windows, and Linux. Specific Node.js versions, platforms, and architecures can be targeted in the packaging process to build just what you need.


## 3. How did you make it work?
1. What mistakes did you make?
    Hardest part was figuring out how to compile a Windows app on a macOS machine. In my testing and review of making an Electron app I installed [Wine](https://www.winehq.org/) to allow me to compile a Windows version of the Electron app. When I went to compile the solution with PKG it just worked to create a Windows version. So, I can't say for sure what is required to build the Windows version from a macOS machine.
    Outside of this it is just a matter of installing the package globally to run 
2. Demo, if you must
    No demo. Examples of package.json setup and commands to run.

## 4. Where to get started?
PKG is on Github here: https://github.com/zeit/pkg
## 5. Wrap it up!

[Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)