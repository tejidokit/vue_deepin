<br />
<p float="left">
<img src="https://user-images.githubusercontent.com/42762293/191895178-349dce0b-2f58-4edb-8494-575e98ac8a7d.svg" width="100" height="100"> <img src="https://user-images.githubusercontent.com/42762293/191897198-d3dc5a76-ae9b-46f8-bf33-087f6f27e591.svg" width="100" height="100">
</p>


<br />


# Set up a Vue web development environment using Deepin

<br />

 :warning: WARNING          


Do **NOT** use the ```sudo su``` command on the terminal, doing so will mess with the node files that are needed to run in your distro
<br>
and this guide will not work.


<br />
<br />

#### Update the system then run the following commands to remove potentially old versions of Node and avoid potential problems in our fresh install

```css
sudo apt update
```

```css
sudo apt upgrade
```

```css
sudo apt-get purge --auto-remove nodejs
```

```css
node -v
```

 > command 'node' not found but can be installed with sudo apt install nodejs


<br />
<br />


#### Install git
```css
sudo apt install git
```

```css
git --version
```

<br />

#### Link your git to your github repo, more details [here](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-config).

```css
git config --global user.email "your_email@example.com"
```

```css
git config --global user.name "spongebob"
```


<br />
<br />

#### Install curl using the github repo below then install the Node Version Manager

```css
sudo apt install curl
```

```css
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```



<br />
<br />



| :exclamation:    | CLOSE and REOPEN the terminal then type, do not proceed to the next steps if you do not CLOSE then REOPEN the terminal.|
|---------------|:------------------------|

<br />
<br />

#### Check what Node Version Manager is installed to confirm that the installation was successful.
```css
nvm --version
```

> 0.38.0

| By the time of this writing, 0.38.0 was the latest version  |
|-----------------------------------------|

<br />
<br />



#### Check what Node Version Manager Long Term Support is available then install it using the commands below.
```css
nvm ls-remote
```

```css
nvm install --lts
```

> Installing latest LTS version.
> v16.17.0 is already installed.
> Now using node v16.17.0 (npm v8.19.2)


| By the time of this writing, in Sept, 2022, these were the most updated versions so yours might be different if you are reading this guide from the future |
|-----------------------------------------|

<br />
<br />

#### Install the LTS or Long Term Support version of NVM.

```css
nvm use --lts
```

> Now using node v16.17.0 (npm v8.19.2)

| Installing the LTS version is more stable and less prone to bugs |
|-----------------------------------------|

<br />
<br />


### Start your Vue project using the Vite build tool
```css
npm create vite@latest
```
<br />
<br />

#### After following the Vite set up on the terminal your terminal should have have a similar output below among other strings of text

> ➜ Local: http://localhost:5173/

<br />

   


| :exclamation:    | If your default browser has not pulled up a webpage a showing a Vue + Vite page, simply press ctrl button on your keyboard + left mouse button on the local host like like the one above (http://localhost:5173/) to go to the Vue + Vite webpage|
|---------------|:------------------------|

<br />
<br />

#### While the Vue + Vite starter page is running, find your project file, right click and open with VS Code to start coding

or

#### Click the  <img src="https://user-images.githubusercontent.com/42762293/191899713-7d986d32-8779-4d87-9f5c-f65528e75a90.svg" width="30" height="30">    button on the same terminal to create another tab, then type the command below to open VS Code in the same file that you created.
```css
code .
```
<br />
<br />

### To exit the terminal type the command below
```css
exit
```
<br />
<br />

#### Done!
#### Congratulations. :tada:

#### 

<br />

***


:bulb:    To open your project file again, find the folder and then right click -> open with -> Visual Studio Code then type the command
on your Visual Studio Code terminal

```css
npm run dev
``` 
***
<br />
<br />
<br />

:beetle: :beetle: :beetle: :beetle: :beetle: :beetle: :beetle: :beetle: :beetle: :beetle: :beetle:
### Potential problems: 

Node and npm still showing after uninstalling it with the commands 

 ```css
sudo apt-get purge --auto-remove nodejs.
```
<br />

#### Solution: 
```css
nvm deactivate
```
```css
nvm uninstall 16.17.0 
```
| This command will force NVM to uninstall the version that you installed, in our case it is the version 16.17.0|
|-----------------------------------------|
