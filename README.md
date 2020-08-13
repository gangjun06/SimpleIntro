# Simple Intro
simple theme for hugo

![intro](imgaes/img1.png)

# Live Demo
https://gangjun06.github.io/hugo-theme-simple-intro-demo

[Demo Source Code](exampleSite)

# Get Started

```bash
hugo new site <site-name>
cd <site-name>
git submodule add https://github.com/gangjun06/hugo-theme-simple-intro themes/simple-intro
# Apply config
hugo serve -D
```

config.toml
```toml
baseURL = "/"
languageCode = "en-us"
theme = "simple-intro"
title = "Title"

[params]
    mainbg = "backroundImage Path"
    name = "Your Name"
    mainTitle = "Header Title"
    mainText = "Header Text"

[menus]
    [[menu.main]]
        identifier = "about"
        name = "About"
        url = "#about"
    [[menu.main]]
        identifier = "skills"
        name = "Skills"
        url = "#skills"
    [[menu.main]]
        identifier = "projects"
        name = "Projects"
        url = "#projects"
    
```

data/home/about.toml
```toml
title = "about title"

text = """
about text
"""

[[link]]
    icon = "fontawesome icon"
    link = "#"
```

data/home/project.toml  
```toml
[[list]]
    title = "project name"
    image = "Project image"
    text = """
    project description
    """
```

data/home/skills.toml
```toml
[[list]]
    name = "lang Name"
    icon = "lang Icon"
    text = """
        skill text
    """
```
