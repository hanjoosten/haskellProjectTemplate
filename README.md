# myHaskellProject

This repository is meant to hold a template to get anyone up to speed with a development environment for [Haskell](https://www.haskell.org/) projects.


## How to use?

There are two ways that this template could be used, depending on your needs. You could either open it as a [codespace](https://github.com/features/codespaces) or clone it into a repository of your own and use it in a local vscode environment.

Head over to the [template repo](https://github.com/hanjoosten/haskellProject) and click the green button `Use this template`, and make your choice:

### Create a new repository

This choice will do what it says: It will create a copy of the template repo. You can use this copy to start your Haskell journey. This is done as you would do with any other git repo: Clone it onto your machine and start hacking. For best experience, I strongly suggest you use vscode as your IDE, for the configuration of this repo uses its [development container](https://containers.dev/) functionality. 

### Open in a codespace 

This choice doesn't differ a lot from the previous. It copies the template repo to a repo of yourself, but you work in the cloud. Also, it is less dependant on whatever your own machine looks like.

## Test your installation

Whatever choice you made above, effectively you will now have a repo of your own to play with. I assume that you use vscode in both cases. 

### Happy flow
It will have taken a while (expect 15 to 20 minutes), the first time vscode was launched with your new repo. If it is ready, open a terminal, and type 

~~~.bash
ghc --version
~~~

It should response with: 

~~~
The Glorious Glasgow Haskell Compilation System, version 9.2.8
~~~

### Not so happy flow
If for whatever reason you don't have ghc, try to [rebuild the container](https://docs.github.com/en/codespaces/developing-in-a-codespace/rebuilding-the-container-in-a-codespace). In all cases I have seen until now, this helped. 


## Get ready to start with Haskell

As your environment is good to go, let's have a look at the project structue. There are several directories:

* `app`: It holds the Main endpoint.
* `src`: This is where most of your code will reside.
* `test`: This is where your test code will be.

In the root directory, there are some files that are standard in a Haskell project:
* `Setup.hs` contains build info. Normally there is no need to change it.
* `package.yaml` contains info about your project and it's required dependencies.
* `stack.yaml` contains aditional info for the `stack` build system.

Happy Haskelling!
