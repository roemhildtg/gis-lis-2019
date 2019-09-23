---
marp: false
title: Automating Workforce assignments with Python Notebooks and Jenkins Automation Server
description: Hosting Marp slide deck on the web
theme: uncover
class:
    - lead
    - invert
paginate: true
_paginate: false
---

![bg](./assets/gradient.jpg)

# Automating Workforce assignments with Python Notebooks and Jenkins Automation Server

Presented By: Gregg Roemhildt
https://github.com/roemhildtg/

<style scoped>a { color: #eee; }</style>

---

# About Me

 - Web Developer @ [WSB](https://wsbeng.com)
 - Python, Javascript (NodeJS, ES6)
 - Web GIS (Workforce, Survey123, Enterprise, PostGIS)

---

 # Why Automate Workforce?

 - Reduce errors/provide consistency
 - Save time
 - Standardize assignments data

```python
# Example of a custom assignment
workforce.Assignment(
    description = f'{contact_name}, {contact_phone}',
    location = f'Inspection at {project_name} - Project #{project_number}', 
    due_date = today + datetime.timedelta(hours=12),
    # .....
)
```
---

# Components
 - Workforce for ArcGIS
 - [Jupyter Notebooks](https://jupyter.org/), Python, & [ArcGIS Python API](https://developers.arcgis.com/python/)
 - [Jenkins Automation Server](https://jenkins.io/)

---


# What is Workforce?

Feature layers, Applications, and Integrations

![Workforce](./assets/Workforce.png?)

---

# Python and Jupyter Notebooks

 - Exploratory python scripting
 - Easy to document and explain
 - Converts to executable python script
 - ArcGIS Python API

![Jupyter](./assets/jupyter.svg)

---

## Jupyter Alternatives:
 - PyCharm
 - VSCode
 - ...

## Script Language alternatives

 - ArcGIS REST JS API (node)

---

![Jenkins](./assets/jenkins.jpg)

 - Powerful task automation tool
 - Free and open source
 - Detailed logging
 - Secure credentials
 - Powerful scheduling

---

## Development Overview

![Process](./assets/Process.png)

---

## Python Process

![Python](./assets/Python.png)

---
<!-- class: invert -->

Python Process 2

![FilterLogic](./assets/FilterLogic.png?)

---

### <!--fit--> :question:

---

![bg 40% opacity blur](https://avatars1.githubusercontent.com/u/3993388?v=4)

### Created by Yuki Hattori ([@yhatt](https://github.com/yhatt))

https://github.com/yhatt/marp-cli-example
