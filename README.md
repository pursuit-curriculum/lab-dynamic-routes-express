# Building Dynamic Routes in Express Lab

## Introduction

Here you will build two small projects in one Express server to keep learning express.

## Getting started

- Fork this repo
- `git clone` the forked repository
- `cd` to the directory where you cloned it
- `touch app.js`
- `npm init -y`
  - follow the prompts and confirm settings (this is just practice so it's ok to not
- `npm install express`
- `npm install nodemon --save-dev`

> **Note:** `.gitignore` has already been included and set up for you in this repository. This `.gitignore` is the standard one from GitHub`. When you create a new repository on GitHub, it gives you the option to automatically add `.gitignore`.

## Build a basic Express server

Build a basic express server that has a welcome message at the root route.

## New project name generator

Create a new route that takes three parameters in the URL:

- verb
- adjective
- noun

so that if the url is

http://localhost:8888/jumping/joyous/jellybean

The response will be

```
Congratulations on starting a new project called jumping-joyous-jellybean!
```

## 99 Little Bugs In the Code

```
99 little bugs in the code
99 little bugs
Pull one down
Patch it around
101 bugs in the code
```

### Requirements

- On the home page (`get "/bugs"`), users should see:
  - "99 little bugs in the code"
  - a link that says "pull one down, patch it around"
  - this should link to `/bugs/101`, where the number represents the number of bugs remaining to fix
- When a number is given in the url (`get "/bugs/:numberOfBugs"`), users should see:
  - The number of bugs left in the code (i.e. `101 little bugs in the code`)
  - a link to "pull one down, patch it around", where the href is number of bottles in the parameter plus 2
- If there over 200 bugs left, do not show a link to "pull one down", rather, add a link to start over, which directs the user back to the home page

#### Hints

- You should use an `anchor` tag with an `href` to link to the next 'page'

## Bonus

Start or continue working on Express UFO
