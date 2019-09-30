---
marp: true
title: Automating Workforce with Python Notebooks and Jenkins Automation Server
description: Hosting Marp slide deck on the web
theme: uncover
class:
    - lead
    - invert
paginate: true
_paginate: false
---
<style>

pre {
    font-size: 20px;
}
</style>
<style scoped>
    img {
        background: rgba(255, 255, 255, 0.5);
        padding: 10px;
        border-radius: 15%;
    }
</style>

# Automating Workforce with Python Notebooks and Jenkins Automation Server

Presented By: Gregg Roemhildt
https://github.com/roemhildtg/gis-lis-2019


[![WSB](./assets/wsb.svg)](https://wsbeng.com)

---

# About Me

 - Web Developer @ [WSB](https://wsbeng.com)
 - Python, Javascript (NodeJS, ES6)
 - Web GIS (Workforce, Survey123, Enterprise, PostGIS)

---

# What is Workforce?

Feature layers, Applications, and Integrations

![Workforce](./assets/Workforce.png?)

---

 # Why Automate Workforce?

 * Save time
 * Reduce errors
 * Provide consistent assignments data
 * Our scenario: 
    * 300+ projects
    * Daily inspections
    * 100 + inspectors


---

# Components
 * Workforce for ArcGIS
 * [Jupyter Notebooks](https://jupyter.org/), Python, & [ArcGIS Python API](https://developers.arcgis.com/python/)
 * [Jenkins Automation Server](https://jenkins.io/)

---
<style scoped>
img {
    position: absolute;
    top: 40px;
    right: 100px;
    height: 100px;
}
</style>

![Jupyter](./assets/jupyter.svg)

# Jupyter Notebooks 

 * Exploratory python scripting
 * Easy to document and explain
 * Converts to executable python script
 * ArcGIS Python API

---

![Jenkins](./assets/jenkins.jpg)

 * Powerful task automation tool
 * Free and open source
 * Detailed logging
 * Secure credentials
 * Powerful scheduling
 * Email notifications
 * Automatic cleanup
 * Extendable with plugins

---

## Jenkins in GIS

 * Build your apps
 * Publish services
 * Service Status Checks (are my services up?)
 * Automate tasks

---

### When can tasks be run?

 * Manually
 * Run tasks on a trigger (webhook)
 * Run on a schedule
    * Midnight
    * Once every hour
    * Once every hour at exactly 30 minute mark

---

## Development Overview

![Process](./assets/Process.png)

---

## Python Logic

![Python](./assets/Python.png)

---

## Python Schema
<style scoped>
    img {
        padding:50px;
        background: rgba(255,255,255,0.1);
    }
</style>
![FilterLogic](./assets/FilterLogic.png?)

---

# Development Tips

 * Use a virtual environment for all installed modules
 * Save dependencies to a [`requirements.txt`](https://www.idkrtm.com/what-is-the-python-requirements-txt/) file
 * [Use `.env` files for all configuration parameters](https://preslav.me/2019/01/09/dotenv-files-python/)
 * Do not save credentials to your script files or repository

requirements.txt:
 ```
arcgis==1.6.2.post1
Shapely==1.6.4.post2
environs==6.0.0
 ```


---

# Jenkins Tips

 * Don't be intimidated
 * Use the question mark buttons
 * Read the docs
 * Check out the plugins
    * [Generic webhook plugin](https://wiki.jenkins-ci.org/display/JENKINS/Generic+Webhook+Trigger+Plugin)
    * [ShiningPanda Plugin](https://wiki.jenkins.io/display/JENKINS/ShiningPanda+Plugin) - Automatically sets up virtual environments for your tasks

---

## [Demo - Jupyter](http://localhost:8888/tree)
 - Jupyter and ArcGIS API comes preinstalled with Pro
 - Can also be easilly installed using pip

```bash
# create our custom environment
# packages we install will live here in development
virtualenv env
# *nix, git bash:
source env/Scripts/activate
# On windows instead run 
.\env\Scripts\activate.bat

# install any modules we need in our notebook
#pip install <module name> <module name...>
pip install arcgis Shapely jupyter environs

# run the notebook program
jupyter notebook
```

---

# Interacting with code

 - Run `Shift + Enter` to run a cell
 - Get the result by simply your cell with a variable 

![Jupyter PNG](./assets/Jupyter1.png)

---


![Jupyter PNG](./assets/Jupyter2.png)

----

# Demo - Jenkins

 1) Configure credentials (Git, ArcGIS, etc)
 2) Configure config files (Parameters for script)
 3) Configure tasks (builds)



---

### <!--fit--> :question:

---
<!-- class: default  -->

## Thank you!

Gregg Roemhildt
groemhildt@wsbeng.com



View this presentation at:
https://github.com/roemhildtg/gis-lis-2019

[![WSB](./assets/wsb.svg)](https://wsbeng.com)