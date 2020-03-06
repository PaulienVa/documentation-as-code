name: inverse
layout: true
class: center, middle, inverse
---

.title-slide[
# Applying your coding practices to your documentation
By Kris Geusenbroek and Paulien van Alst
]
.remark-slide-content.img-right-full.inverse[
![](./images/new-developer-docs.jpg)]

---
layout: false

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
- people maintaining the docs left the project
]
--
.right-column[
- people left the project
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
- architect
]  

--
.right-column[
- developers
]
--
.right-column[
- (business) analysts
]

--
.right-column[
- UX designers
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
- architect: .red.bold[ keep track of their drawings ]
]
--
.right-column[
- developers: .red.bold[ stay in the codebase ]
]
--
.right-column[
- (business) analysts: .red.bold[ easy accessible and editable documentation ]
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
- user friendly editor
- lots of plugins
    ]
   .cons[
- bad search 
- far, far away from the code base
 ]
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
 - Architectural drawings: Draw.io
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
.left-column[# Solution
   ### Mkdocs
   ]
--
.right-column[
- known from the python world
]
--
.right-column[
- easy set-up
]
--
.right-column[
- everything in markdown!
  - codebase compliant
  - git clients have nice editors
]
--
.right-column[
- standard themes
]
--
.right-column[
- lots of plugins (active community)
  - coding highlight
  - code snippets
  - very good search
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
- each repository has its own documentation
]
--
.right-column[
- one overall project
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
- use of a pipeline for releasing
]
---

.left-column[# Solution
   ### Mkdocs
   ### Git
   ### Git submodules
   ### Gitlab editor
   ### Docker container
   ]
.right-column[
- deployable!
]
---
name: inverse
layout: true
class: center, middle, inverse
---
# How does it look like? 
## Code example!
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