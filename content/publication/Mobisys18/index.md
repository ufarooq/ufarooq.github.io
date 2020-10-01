---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "RuntimeDroid: Restarting-Free Runtime Change Handling for Android Apps"
authors: [Umar Farooq, Zhijia Zhao]
date: 2018-18-06T15:31:18-07:00
doi: "10.1145/3210240.3210327"

# Schedule page publish date (NOT publication's date).
publishDate: 2018-06-01T15:31:18-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Proceedings of the 16th Annual International Conference on Mobile Systems, Applications, and Services"
publication_short: "MobiSys'18"

abstract: "Portable devices, like smartphones and tablets, are often subject to runtime configuration changes, such as screen orientation changes, screen resizing, keyboard attachments, and language switching. When handled improperly, such simple changes can cause serious runtime issues, from data loss to app crashes.
This work presents, to our best knowledge, the first formative study on runtime change handling with 3,567 Android apps. The study not only reveals the current landscape of runtime change handling, but also points out a common cause of various runtime change issues -- activity restarting. On one hand, the restarting facilitates the resource reloading for the new configuration. On the other hand, it may slow down the app, and more critically, it requires developers to manually preserve a set of data in order to recover the user interaction state after restarting.<space><space>

Based on the findings of this study, this work further introduces a re starting-free runtime change handling solution -- RuntimeDroid. RuntimeDroid can completely avoid the activity restarting, at the same time, ensure proper resource updating with user input data preserved. These are achieved with two key components: an online resource loading module, called HotR and a novel UI components migration technique. The former enables proper resources loading while the activity is still live. The latter ensures that prior user changes are carefully preserved during runtime changes.<space><space>

For practical use, this work proposes two implementations of RuntimeDroid: an IDE plugin and an auto-patching tool. The former allows developers to easily adopt restarting-free runtime change handling during the app developing; The latter can patch released app packages without source code. Finally, evaluation with a set of 72 apps shows that RuntimeDroid successfully fixed all the 197 reported runtime change issues, meanwhile reducing the runtime change handling delays by 9.5X on average."

# Summary. An optional shortened abstract.
summary: "In Android systems, configuration changes, such as screen orientation changes, screen resizing, keyboard attachments, and language switching, are typically handled by application restarting, which, due to poor coding practices, can result in user data loss to app crashes. RuntimeDroid describe a restart-free runtime that avoids the need for application restarting while ensuring proper resource updating and user data preservation."

tags: []
categories: []
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf:
url_code: "https://github.com/ufarooq/RuntimeDroid"
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:
url_other_award: "https://beta.sigmobile.org/articles/research-highlights/"
url_conference_award: "https://www.sigmobile.org/mobisys/2018/papers/"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
