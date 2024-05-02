---
sticker: lucide//laptop-2
---


[[Medcross Requirements]],
[[Pseudocode.canvas|Pseudocode]]

The app is to create a crossword game to serve as a fun pastime for med students and personell, and hopefully help them learn while at it  
  
Going for the simplest solution of architecture, with **11ty(SSG)**, and **web components** with the **flamethrower router**(a router for multi-page apps built by fireship) to help make this feel as fast and smooth like a single page application, while giving the elegance and simplicity of managing data with **markdown and nunjucks**, and **NetlifyCMS** for peak authoring experience  
  
  
New Proposed Stack:  
**astro** as the architecture, so that I can use all kinds of component frameworks.  
  
  
  
basic requirements  
- [x]  a crossword component that allows for playing a classic crossword puzzle  
- [x]   save the progress and can resume the puzzle later **(resumabilty)**  
- [x]   give a gui for crossword creation  
- [ ]   docs for the features of the app  
  
features to build on top of an actual cross  
- [x]  add categories to the crosswords 
- [x]   allow users to favorite crosswords  
- [x]   have a mode to ask the crossword as german questions.    
  
Optional Features  
-  [ ]   leaderboard for points? most likely not, too complicated, cause I want to keep all of the user data on-device; no persistent DB  
-  [ ]   building a desktop app with this; not if I want to update the data and keep it in sync, unless there's like a background function for getting the most up-to-date data  
-  [ ]   a component that just drops on the page periodically, just to keep users on their toes, which is one **optional** german-question quiz; some people may not like the jumping around (layout shift)
- [ ]   share your points to social-media platforms with like a picture and some text linking to the app  
  
  
app architecture  [[Navigation]]
- [x]  home page with hero, latest crosswords  [[Home Page]]
- [x]  all crosswords  
- [x]  categoried crosswords  
- [x]  create crossword page  
- [ ]  downloads  
- [x]  favorites page  
- [x]  start game page   
  - [x]  crossword mode  
  - [x]  German mode