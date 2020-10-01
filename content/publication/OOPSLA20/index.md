---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "LiveDroid: Identifying and Preserving Mobile App State in Volatile Runtime Environments"
authors: [Umar Farooq, Zhijia Zhao, Manu Sridharan, Iulian Neamtiu]
date: 2020-09-30T15:58:20-07:00
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: 2020-09-30T15:58:20-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Proceedings of the ACM on Programming Languages (PACMPL), Volume 3, Issue OOPSLA, 2020"
publication_short: "OOPSLA'20 "

abstract: "Mobile operating systems, such as Android, expose apps to a volatile runtime environment. For example, app state that reflects past user interaction can be destroyed implicitly, in response to runtime changes (e.g., screen rotation) or high memory pressure. Developers are therefore responsible for identifying that app state affected by volatility and preserving it across app lifecycles. When handled inappropriately, the app may lose state or end up in an inconsistent state when users return to the app.

To free developers from this tedious and error-prone task, this work proposes a systematic solution -- LiveDroid, which automatically and precisely identifies the app state, saves it before the app gets destroyed, and recovers it when users return to the app. LiveDroid consists of: (i) a static analyzer that reasons about data uses to pinpoint the critical data set that capture the user interaction, and (ii) a runtime system that manages the data saving and recovering. We implemented LiveDroid as a plugin in Android Studio and a patching tool for APKs. Our evaluation shows that LiveDroid can be successfully applied to 966 Android apps. A focused study with 36 Android apps shows that LiveDroid identifies app state much more precisely than existing work. As a result, on average, LiveDroid is able to reduce the costs of state saving and restoring by 16.6X (1.7X - 141.1X) and 9.5X (1.1X - 43.8X), respectively. Furthermore, compared with the manual state handling performed by developers, our analysis reveals a set of 46 app state issues due to the incomplete state saving/restoring, all of which can be successfully eliminated by LiveDroid."

# Summary. An optional shortened abstract.
summary: ""

tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf:
url_code: "https://github.com/ucr-riple/LiveDroid"
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

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
