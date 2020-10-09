# Task Two - Architecture

## d032-c3-asynchronous-programming-with-javascript-project-starter

for top level tree

`tree -L 1`

```
├── bin
├── data.json
├── LICENSE
├── node_modules
├── package.json
├── package-lock.json
├── project_notes
├── README.md
└── src
```

nd032-c3-asynchronous-programming-with-javascript-project-starter/src 

 for subsequent levels this example showing 4 levels
 `tree -L 4`
 
 * client - Client side rendering
 * server - Server side rendering
 
```
├── client
│   ├── assets
│   │   ├── javascript
│   │   │   └── index.js
│   │   └── stylesheets
│   │       ├── create.css
│   │       ├── form.css
│   │       ├── home.css
│   │       ├── index.css
│   │       ├── progress.css
│   │       ├── reset.css
│   │       └── results.css
│   └── pages
│       ├── home.html
│       ├── progress.html
│       ├── race.html
│       └── results.html
└── server
    └── index.js
```
    
 ### server/index.js
- [x] Change the port from `3000` to `8080`
- [x] Path for `public`
- [x] Route for `/`
- [x] Route for `/race`

### client/pages/home.html
- [x] Links to CSS
- [x] Displays home page which is shown on load
- [x] Contains button which takes you to race.html onClick `<a class="button" href="/race">Start My Race</a>`

### client/pages/progress.html
- [x] Links to CSS
- [x] Links to  /assets/javascript/index.js
- [x] Displays leadeboard in thr form of a HTML table 
- [x] Contains gas peddle button 
   ```
    <section id="accelerate">
            <button id="gas-peddle">Click Me Fast!</button>
        </section>
    ```
    
### client/pages/race.html
- [x] Links to CSS
- [x] Links to  /assets/javascript/index.js
- [x] Displays form to allow user to select track and racer
- [x] Contains form submit button  `<button class="button" type="submit" id="submit-create-race">Start Race</button>`

### client/pages/results.html
- [x] Links to CSS
- [x] Links to  /assets/javascript/index.js
- [x] Basic template for displaying results, no structure only 2 headers

### client/assets/javascript/index.js

- [x]  Object: store
- [x]  function: document.addEventListener("DOMContentLoaded", function())- wait until the DOM is loaded the call -> onPageLoad() & setUpClickHandlers()
- [ ]  async function: onPageLoad() -> getTracks() & getRacers()
- [x]  function: setupClickHandlers() - eventListener for html form (see diagram??) **diagram needed**
- [ ]  async function: delay(ms) - try/catch setTimeOut()
- [ ]  async function: handleCreateRace() -> renderAt() This async function controls the flow of the race, add the logic and error handling**action required see task ?? for breakdown**
- [ ]  function: runRace(raceID) ?? unsure of this function **action required see task ?? for breakdown**
- [ ]  async function: runCountdown() try/catch to create a delay for DOM to load **action required see task ?? for breakdown**
- [ ]  function: handleSelectPodRacer(target) remove class selected from all racer options **action required see task ?? for breakdown**
- [ ]  function: handleSelectTrack(target) **action required see task ?? for breakdown**
- [ ]  function: handleAccelerate() invoke API to call accelerate() **action required see task ?? for breakdown**

### HTML views
- [ ]  function: renderRacerCars(racers) 
- [ ]  function: renderRacerCard(racer)
- [ ]  function: renderTrackCards(tracks)
- [ ]  function: renderTrackCard(track)
- [ ]  function: renderCountdown(count)
- [ ]  function: renderRaceStartView(track, racers)
- [ ]  function: resultsView(positions)
- [ ]  function: renderAt(element, html) - renders starting UI

### API calls
- [x]  const: const SERVER = 'http://localhost:8080' **action required see task ?? for breakdown**
- [x]  function: getTracks()
- [x]  function:  getRacers()
- [x]  function: createRace(player_id, track_id)
- [x]  function: getRace(id)
- [x]  function: startRace(id)
- [x]  function: accelerate(id)

### Top level overview of game

![Game flow Overview](https://github.com/tastethedream/nd032-c3-asynchronous-programming-with-javascript-project-starter/blob/development/project_notes/images/task2-top-level-diagram.png)







