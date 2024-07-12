# Real-Time Device Tracker
### This project is a real-time device tracker that uses Node.js, Express, Socket.io, and Leaflet.js. The application tracks and displays the locations of connected devices on a map in real-time.

## Prerequisites
Before you begin, ensure you have met the following requirements:

- You have installed Node.js and npm.
- You have a basic understanding of [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript), [Node.js](https://nodejs.org/docs/latest/api/), and [Express](https://expressjs.com/en/5x/api.html).
## Installation
### Clone the repository:

```
git clone https://github.com/your-username/realtime-device-tracker.git
cd realtime-device-tracker
```
### Install dependencies:
```
npm install
```
### Start the server:
```
node app.js
```
### Open your browser and go to:

[http://localhost:3000](http://localhost:3000)

## Project Structure
### The project consists of the following files and directories:

```
realtime-device-tracker/
├── app.js
├── package.json
├── public/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── script.js
└── views/
    └── index.ejs
```
### File Descriptions
- app.js: This is the main server file. It sets up the Express server, integrates Socket.io, and handles client connections and disconnections.

- public/css/style.css: This file contains the CSS styles for the project.

- public/js/script.js: This file contains the client-side JavaScript code that integrates with Socket.io and Leaflet.js for real-time location tracking.

- views/index.ejs: This file contains the HTML template for the application, integrating Leaflet.js for map rendering.

## Usage
- Open the application in your browser.
- Allow geolocation permissions in the browser.
- Open multiple browser tabs/windows to see multiple devices being tracked.
## How It Works
### Server Side:

* The server listens for send-location events from connected clients.
Upon receiving a send-location event, the server broadcasts the location to all connected clients.
* The server also listens for client disconnections and notifies all clients when a user disconnects.
### Client Side:

* The client sends its geolocation to the server using the send-location event.
* The client listens for receive-location events to update the map with the locations of all connected clients.
* The client listens for user-disconnected events to remove the marker of a disconnected client.
## Snapshots
<img src="https://github.com/KhushiRaj23/Real-Time-Device-Tracker-Project/blob/master/image.png" style="height: 50vh; width: 50vw;"/>
<br>
<br>
<img src="https://github.com/KhushiRaj23/Real-Time-Device-Tracker-Project/blob/master/image1.png"  style="height: 50vh; width: 50vw;"/>

## Contributing
**If you have any ideas, suggestions, or improvements, feel free to fork the repository and create a pull request.**

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements
* [Node.js](https://nodejs.org/en)
* [Express](https://expressjs.com/)
* [socket.io](https://socket.io/)
* [Leaflet.js](https://leafletjs.com/)
* [OpenStreetMap](https://leafletjs.com/)

## Author
GitHub: [KhushiRaj23](https://github.com/KhushiRaj23)

## Reference 
* [Sheryians Coding School](https://www.youtube.com/@sheryians)
