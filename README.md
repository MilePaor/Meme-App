# Meme-App

The main idea is to provide a seemless interface for creating memes on web, while I have personally enjoyed creating memes on apps in phones but sometimes you just need a web-app on a big screen. This is the solution to that problem.  

What to contribute? Check the issues section and let me know if you are intresting in contributing in something or reach out to me on [Twitter](https://twitter.com/jai_dewani)

Visit the hosted version [here](https://jai-dewani.github.io/Meme-App/)

## Github actions
If you have already enabled ssh for your GitHub account, you can use that public/private key pair. Else you will need to create a new one.

### create a public/private key

```bash
cd ~/.ssh
ssh-keygen -t rsa -b 4096 -C "$(git config user.email)" -f gh-pages-actions -N ""
```

Don’t forget to replace user.email with your e-mail address. 

You need to insert the public key you have generated into the text-area. Insert Public key of ACTIONS_DEPLOY_KEY for the title input field. Check Allow write access and click on the Add key button.

### view the public key

```bash
cat ~/.ssh/gh-pages-actions.pub
```
Next, up go to the secrets tab and add a new secret key. This is the private ssh key that you generated. You can view it like this. In the name field, add ACTIONS_DEPLOY_KEY
```bash
cat ~/.ssh/gh-pages-actions
```
We have integrated GitHub Actions into your workflow.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm run deploy`

Deploys the project

