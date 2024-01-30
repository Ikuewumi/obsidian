

[[Medcross Requirements]],
[[Pseudocode.canvas|Pseudocode]]

The app is to create a crossword game to serve as a fun pastime for med students and personell, and hopefully help them learn while at it  
  
Going for the simplest solution of architecture, with **11ty(SSG)**, and **web components** with the **flamethrower router**(a router for multi-page apps built by fireship) to help make this feel as fast and smooth like a single page application, while giving the elegance and simplicity of managing data with **markdown and nunjucks**, and **NetlifyCMS** for peak authoring experience  
  
  
New Proposed Stack:  
**astro** as the architecture, so that I can use all kinds of component frameworks.  
  
  
  
basic requirements  
- [ ]  a crossword component that allows for playing a classic crossword puzzle  
- [ ]   save the progress and can resume the puzzle later **(resumabilty)**  
- [x]   give a gui for crossword creation  
- [ ]   docs for the features of the app  
  
features to build on top of an actual cross  
- [ ]  add categories to the crosswords 
- [ ]   allow users to favorite crosswords  
- [ ]   have a mode to ask the crossword as german questions.  
- [ ]   save crossword to device - downloads  
- [ ]   filter for the all crosswords page  
- [ ]   implement a coins system for buying the answer to a word while playing the game  
- [ ]   points system  
- [ ]   make a progressive web app that has some offline functionality  
  
  
Optional Features  
-  [ ]   leaderboard for points? most likely not, too complicated, cause I want to keep all of the user data on-device; no persistent DB  
-  [ ]   building a desktop app with this; not if I want to update the data and keep it in sync, unless there's like a background function for getting the most up-to-date data  
-  [ ]   a component that just drops on the page periodically, just to keep users on their toes, which is one **optional** german-question quiz; some people may not like the jumping around (layout shift)
- [ ]   share your points to social-media platforms with like a picture and some text linking to the app  
  
  
app architecture  [[Navigation]]
- [ ]  home page with hero, latest crosswords  [[Home Page]]
- [ ]  all crosswords  
- [ ]  categoried crosswords  
- [ ]  create crossword page  
- [ ]  downloads  
- [ ]  favorites page  
- [ ]  start game page   
  - [ ]  crossword mode  
  - [ ]  German mode