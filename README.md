[![Website Badge](https://img.shields.io/badge/-kira_porter_com-e34f26?style=flat-square&logo=Portfolio&logoColor=white&link=https://github.com/kierxin)](https://github.com/kierxin)
[![AngelList Badge](https://img.shields.io/badge/-kira's_angel-e4405f?style=flat-square&logo=AngelList&logoColor=white&link=https://github.com/kierxin)](https://github.com/kierxin)
[![Linkedin Badge](https://img.shields.io/badge/-kiraporter-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://github.com/kierxin)](https://github.com/kierxin)
[![Gmail Badge](https://img.shields.io/badge/-kierxin@gmail.com-d14836?style=flat-square&logo=Gmail&logoColor=white&link=mailto:kierxin@gmail.com)](mailto:mail@kierxin@gmail.com)

***

## Hello! 😎 Thanks for stopping by!

#### I'm Kira. A bit about me...
  
* ```ruby
  education = {
    coding: { "App Academy 💻" => 
        ["SWE Full Stack Bootcamp", "Jun 2021 - Oct 2021"] },
    undergrad: { "UMass Amherst 🎓" => 
        ["BBA Operations Management", "Sep 2017 - May 2021"] }
  }
  ```
* ```sql
  SELECT opportunity
    FROM jobs 
    WHERE location IN ('NYC', 'Boston', 'Philly', 'Bay Area');
  ```
* ``` javascript
  const otherInterests = ["dancing 💃", "hiking 🌲", "writing ✍", "food 🌮🍣🍄🥗🍜🧀"];
  ```


## My Projects  

### The Coolony Game: [Live Demo](https://kierxin.github.io/The-Coolony-Game/ "https://kierxin.github.io/The-Coolony-Game/"), [Repo](https://github.com/kierxin/The-Coolony-Game "https://github.com/kierxin/The-Coolony-Game")

> Built with vanilla JS, HTML, and SCSS, this is an ant-themed, idle-clicker-esque game that I built for the week-long JavaScript Project for App Academy. It's a front-end app where the user delegates tasks to the ants in the colony, gathering resources and discovering more tunnels, while ensuring that their ants don't starve. 

> The game board is a two-dimensional array of tile objects, which each have properties pertaining to visibility, ways in which the user can interact with the tile, and which ants are currently assigned to do a task at the tile. When the game begins, the user is given one of three 10x6 starter boards. A randomly created 10x14 board is appended to that, based on a predetermined number of each type of tile that should appear on the board. The array is then translated into the DOM (document object model) as a 1D array of 200 tiles. Each tile's apperance is manipulated based on its classList (CSS class). By doing certain game tasks, the user can trigger event listeners that add or remove a tile's classes.

> The game runs on a setInterval loop, which I currently have set to 500 milliseconds. After the board has been rendered onto the DOM and a player instance has been created (along with two ants), an update function is called at each interval, which in turn calls several functions for checking which ants have completed a task; updating corresponding resources based on time completion; re-displaying each ant's status and the player's resources; decaying the ants' energy; and decrementing the remaining time each ant must spend on its current task.

> The primary way the user interacts with the game (as it stands now) is through the Ants List icon to the right of the game window. Click events on the icon open up a modal, which lists the player's ants by ID, along with each ant's status. Clicking on a list item toggles the visibility of a dynamically-rendered HTML form that allows the user to assign the ant a new task if it is not already occupied. Since the project doesn't have a backend, the form isn't submitted anywhere. Instead, when the user selects a task from the dropdown options, an 'onchange' event is fired, which updates the player instance's properties to reflect which ant has most recently been clicked on in the list. When the user clicks the submit button, another event fires to parse value of the selected option and update the task and task duration properties of the player's most recently selected ant. 

> Another feature of the game is the ability for the player to dig more tunnels, discovering new tiles. This feature is broken into two parts: choosing a new excavation site and assigning an ant to dig at that site. The bulk of the logic happens in part one, where the player must choose a tile to establish their excavation site at and spend some of their accumulated resources. To choose a tile to excavate, the player clicks the 'build mode' icon to the right of the game window. An excavation class is added to each of the available tiles (clicking the icon again toggles the class back off). Available tiles include all tiles that are undiscovered which directly border an already discovered tile. When the player clicks on one of the available tiles, a box pops up prompting confirmation, after which resources are deducted or else the window alerts that there are insufficient resources. 

> One of the biggest challenges in the project was updating the 2-D JavaScript array representation of the board (which the player never sees) alongside the corresponding 1-D DOM representation of the board (the one that the player does see). While it's possible to iterate through DOM objects' children (equivalent to an array's elements), it is not exactly the same as iterating through an array. Add that to the fact that each tile has two different indices (one for the JS and one for the DOM) and you end up with a lot of separate looping going on behind the scenes.

> Going forward, I'd like to allow users to click on a tile to view the ants currently doing a task on that tile and a form through which idle ants could be assigned to that tile. I'd also like to implement the ability for the player to add more ants (the nursery). Graphics-wise, I'm proud of what I made for the project (all of the graphics/art) but I'd love to add some texture to the tiles and maybe even play around with the parallax scrolling effect that I didn't get around to trying out. And maybe I'll look to make an algorithm that finds the shortest path from an origin tile to a destination tile, so that an ant can appear to run between the tiles when a task has been assigned.

### Project 2: [Live Demo](https://github.com/kierxin "https://github.com/kierxin"), [Repo](https://github.com/kierxin "https://github.com/kierxin")
> Descrip
