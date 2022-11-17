# What I am doing using Git

In the **Assignment #4 demo-git**, I'll be representing on what I am doing so far using Git. I'm doing a simple web-development workflow:

<br>

### **First**

I'm creating index.html file and record the changes in the repository using command below, <br> Proof: `bfceac6` create index.html

```sh
git add index.html
git commit -m "create index.html"
```

<br>

### **Second**

I'm adding app logic using javascript and record the changes in the repository using command below, <br> Proof: `707b478` create index.html

```sh
git add app.js
git commit -m "add app logic"
```

<br>

### **Third**

I'm adding styles using CSS and record the changes in the repository using command below, <br> Proof: `af42681` create index.html

```sh
git add styles.css
git commit -m "add basic styles"
```

<br>

### **Fourth**

I'm changing background color of the web-page using CSS and record the changes in the repository using command below, <br> Proof: `50da501` create index.html

```sh
git add styles.css
git commit -m "change background color on body"
```

<br>

### **Fifth**

In this section, I'm trying to add a branch called 'crazycolors'. In this branch I'm delete all the previous css styles and replace it with css styles from other source. With this method, I can compare the styling of previous repository with the new styling in _crazycolors_ branch.

```sh
git branch crazycolors
git checkout crazycolors
git add styles.css
git commit -m "add animated bg"
```

<br>

### **Sixth**

Because I like the new css styling in the 'crazycolors' branch therefore I'm merging repository in branch with repository in main, using command below,
Proof: `8531ef0`

```sh
git merge crazycolors
```

---

<br>

## Push to github repository

I'm using SSH instead HTTPS. To generate the SSH keys and connect it to GitHub account using command in the home folder

```sh
cd ~
ssh-keygen
```

After I obtained the SSH keys, I add it in my GitHub account. <br><br> Before I can push the file I created in the local repository, I need to make GitHub repository called: demo-repository. In this repository, I copy the respective ssh keys of demo-git repository in order to push the file I created in the local repository. Using command below to push:

```sh
git remote add origin git@github.com:jeffrymahbuubi/demo-git.git
git push origin main
```
