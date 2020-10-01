# Task 3 API Calls

## API Endpoints

To complete the project you must first create the calls to the API. These will all be fetch requests, and all information needed to create the request is provided in the instructions. The API calls are all at the bottom of the file: `src/client/assets/javascript/index.js.`

Below are a list of the API endpoints and the shape of the data they return. These are all of the endpoints you need to complete the game. Consult this information often as you complete the project:

**[GET] api/tracks List of all tracks**

* id: number (1)
* name: string ("Executioner")
* segments: number[] ([87,47,29,31,78,25,80,76,60,14....])

[**GET] api/cars List of all cars**

* id: number (3)
* driver_name: string ("Anakin Skywalker")
* top_speed: number (500)
* acceleration: number (10)
* handling: number (10)

**[GET] api/races/${id} Information about a single race**

* status: RaceStatus ("unstarted" | "in-progress" | "finished")
* positions object[] ([{ car: object, final_position: number (omitted if empty), speed: number, segment: number}])

**[POST] api/races Create a race**

* id: number
* track: string
* player_id: number
* ncars: Cars[] (array of cars in the race)
* results: Cars[] (array of cars in the position they finished, available if the race is finished)

**[POST] api/races/${id}/start Begin a race**

Returns nothing

**[POST] api/races/${id}/accelerate Accelerate a car**

Returns nothing

To complete the race logic, find all the TODO tags in index.js and read the instructions.

