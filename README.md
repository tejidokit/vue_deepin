# vue_deepin
Step by step guide on setting up a Vue Web Development environment using Deepin Linux

```css
sudo su
```
``` Enter your password ```

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

```css
sudo apt install git
```

```css
git --version
```
#### Link your git to your repo | more details [here](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-config).

```css
git config --global user.email "your_email@example.com"
```

```css
git config --global user.name "spongebob"
```
#### Install curl to instal 3rd party github repo

```css
sudo apt install curl
```

```css
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

#### Close and reopen the terminal

```css
nvm --version
```

> 0.38.0

#### By the time of this writing, 0.38.0 was the latest version

```css
nvm ls-remote
```

```css
nvm install --lts
```

> Installing latest LTS version.
> v16.17.0 is already installed.
> Now using node v16.17.0 (npm v8.19.2)

#### By the time of this writing, in Sept, 2022, these were the most updated versions so yours might be different if you are from the future

```css
nvm use --lts
```

> Now using node v16.17.0 (npm v8.19.2)

#### Do **not** use npm init vue@latest. It doesn't work in my Linux machines, but try substituting "init" with "create", see if it works 

```css
npm create vite@latest
```

#### After following the Vite set up on the terminal your terminal should have have a similar output below among other strings of text

> ➜ Local: http://localhost:5173/

#### If your default browser has not pulled up a webpage a showing a Vue + Vite page, simply press ctrl button on your keyboard + left mouse button on the local host like like the one above (http://localhost:5173/) to go to the Vue + Vite webpage

#### While the Vue + Vite starter page is running, find your project file, right click and open with VS Code to start coding

#### Done!
#### Congratulations.
