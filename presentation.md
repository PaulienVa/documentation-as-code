name: inverse
layout: true
class: center, middle, inverse
---

.title-slide[
# Applying your coding practices to your documentation
By Kris Geusebroek and Paulien van Alst
]
.remark-slide-content.img-right-full.inverse[
![](./images/new-developer-docs.jpg)]

---
layout: false

# Do you all know the "architecture picture on the wall?"

.remark-slide-content.fifty[![](./images/software-architecture-on-wall.png)]

.footnote[https://res.infoq.com/articles/agile-software-architecture-sketches-NoUML/en/resources/1big.png]

---

.left-column[ # Who are we ?]
.remark-slide-content.presentation[![](./images/barcoding_ov.png)] 
.right-column[
### Paulien van Alst - @PaulienVanAlst
.job-description[- Podcaster at BarCoding]
.job-description[- Software engineer @OpenValue]
]
--
.right-column[### Kris Geusebroek]
.right-column[Data Engineer @GoDataDriven]
.remark-slide-content.presentation2[![](./images/go-data-driven.png)] 

---
.left-column[# Current project
### Introduction
]
--
.right-column[
- FIOD (Fiscal Investigation Services)
]
--
.right-column[
- Started two years ago ]
--
.right-column[
- Back-end: Microservices (each in one repository)
]
--
.right-column[
- Front-end: React application
]
--
.right-column[
- User interface design by UX designer
]
--
.remark-slide-content[![](./images/agile-no-docs.jpg)]
---

name: inverse
layout: true
class: center, middle, inverse
---
# Problem: Big team switch
---
layout: false
.left-column[# Team switch
]

.right-column[
- People maintaining the docs left the project
]
--
.right-column[
- People left the project
]
--
.right-column[
 ![](./images/substitue.jpeg)
]

---
name: intervention
layout: true
class: center, middle, intervention
---

# Outdated documentation 
# is worse
# than no documentation at all!

---
name: inverse
layout: true
class: center, middle, inverse
---

.left-column.inverse[# Current project
### Introduction
### Challenge
]
--
.vertical-middle[
## How to get back on track with documentation?

# and

## Make sure we will keep it up to date
]
---
layout: false


.left-column[# Solve the challenge
### Who?
]
--

.right-column[
Who is reading and writing documentation?
] 
--

.right-column[
- Architect
]  

.right-column[
 .remark-slide-content.fifty[![](./images/draw.io_drawing.jpg)]
]

---
.left-column[# Solve the challenge
### Who?
]

.right-column[
Who is reading and writing documentation?
] 
.right-column[
- Developers
]
.right-column[
 .remark-slide-content.fifty[![](./images/markdown-intellij.png)]
]
---
.left-column[# Solve the challenge
### Who?
]

.right-column[
Who is reading and writing documentation?
] 
.right-column[
- (Business) Analysts
 .remark-slide-content.fifty[![](./images/word-screenshot.jpg)]
]

---
.left-column[# Solve the challenge
### Who?
]

.right-column[
Who is reading and writing documentation?
] 
.right-column[
- UX designers
]

.right-column[
 .remark-slide-content.fifty[![](./images/sketch-logo.png)]
]

---
.left-column[# Solve the challenge
   ### Who?
   ### What?
   ]
--
.right-column[
What do they prefer?
]   
.right-column[
- Architect: .red.bold[ keep track of their drawings ]
]
--
.right-column[
- Developers: .red.bold[ stay in the codebase ]
]
--
.right-column[
- (Business) Analysts: .red.bold[ easy accessible and editable documentation ]
]
--

.right-column[
- UX designers: .red.bold[ writing documentation for the tech team AND for the users ]
]


---
.left-column[# Standard solutions
]

.right-column[
- Confluence: 
   .pros[
- User friendly editor
- Lots of plugins
    ]
   .cons[
- Bad search 
- Far, far away from the codebase
 ]
]  
--
.right-column[
 - README.md in the repositories
]
--
.right-column[
 - Word documents for user documentation to generate PDF
 ]
 
--
.right-column[
 - Partial feature documentation in Jira, partially in Confluence
]
--
.right-column[
 - Architectural drawings: (outdated) picture on the wall
 ]
 
--
.right-column[
 .red.bold[-> All different systems solving the documentation challenge]
]

---
name: inverse
layout: true
class: center, middle, inverse
---

# Let's solve this!
## One solution for all

---
layout: false

.left-column[# Requirements
]

.right-column[
- Documentation next to the codebase
]
--

.right-column[
- Easily editable for non-technical users
]
--

.right-column[
- Version controlled
]
--

.right-column[
- Deployable
]
--
.right-column[
- HTML / PDF as an output
]


---
layout: false
.left-column[# Solution
   ### Mkdocs
   ]
--
.right-column[
- Known from the python world
]
--
.right-column[
- Easy set-up
]
--
.right-column[
- Everything in markdown!
  - codebase compliant
  - git clients have nice editors
]
--
.right-column[
- Standard themes
]
--
.right-column[
- Lots of plugins (active community)
  - coding highlight
  - code snippets
  - very good search
  - plugin for different outputs
  ]
---

.left-column[# Solution
   ### Mkdocs
   ### Git
]
.right-column[
- Version control
]
--
.right-column[
- History tracking
]
---

.left-column[# Solution
   ### Mkdocs
   ### Git
   ### Git submodules
   ]
.right-column[
- Each repository has its own documentation
]
--
.right-column[
- One overall project
]
--
.remark-slide-content.presentation[
![](./images/explanation-setup/overview-submodules.png)
]

---

.left-column[# Solution
   ### Mkdocs
   ### Git
   ### Git submodules
   ]
.right-column[
- Each repository has its own documentation
]
.right-column[
- One overall project
]

.remark-slide-content.presentation[
![](./images/explanation-setup/overview-submodules2.png)
]

---

.left-column[# Solution
   ### Mkdocs
   ### Git
   ### Git submodules
   ### Gitlab (editor)
   ]
.right-column[
- User friendly editor
]
.right-column[
- Use of a pipeline for releasing
]


.remark-slide-content.twenty[![](./images/explanation-setup/gitlab-ui.png)]

---

.left-column[# Solution
   ### Mkdocs
   ### Git
   ### Git submodules
   ### Gitlab editor
   ### Docker container
   ]
.vertical-middle.small-right-column[
deployable!
]
.remark-slide-content.image-center[![](./images/docker-logo.png)] 
---
name: inverse
layout: true
class: center, middle, inverse
---
# How does it look like? 
## Code example!
---
layout: false
class: center, middle

# And the UX flow ?
---
.left-column[# UX flow
]

.right-column[
 - UX documentation for tech people
 - UX documentation for users (a bit less than the above)
 
 - Gitlab pipeline will result in both:
        - HTML website (as the microservices/libraries)
        - PDF document (for the users)
]
---
layout: false

.left-column[# Conclusion
]

.right-column[
- UX’er very happy
]
--
.right-column[
- Dev's also happy
]
--
.right-column[
- Git submodules can be annoying (sometimes)
]
--
.right-column[
- We still need a cheet sheet for formatting
]
--
.right-column[
- We constructed a sustainable and stable base for our docs
]