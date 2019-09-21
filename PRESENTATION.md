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

 - Web Developer @ WSB
 - Python, Javascript (NodeJS, ES6)
 - Web GIS (Workforce, Survey123, Enterprise, PostGIS)

---


![bg](#123)
![](#fff)

# About You



---

![bg](#fff)
![color](#123)
# Composition of Workforce Projects

![Workforce](./assets/Workforce.png)

---

 # Why Automate Workforce?

 - Reduce errors/provide consistency
 - Customize assignments
 - Save time

```python
# create assignment due in 12 hours
workforce.Assignment(
    description = f'{contact_name}, {contact_phone}',
    location = f'Inspection at {project_name} - Project #{project_number}', 
    due_date = today + datetime.timedelta(hours=12),
    # .....
)
```
---

## Development Process

![Process](./assets/Process.png)

---

## Python Process



---

### <!--fit--> :ok_hand:

---

![bg 40% opacity blur](https://avatars1.githubusercontent.com/u/3993388?v=4)

### Created by Yuki Hattori ([@yhatt](https://github.com/yhatt))

https://github.com/yhatt/marp-cli-example
