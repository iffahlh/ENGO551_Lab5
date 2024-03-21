# ENGO551_Lab5
This is a simple web application that uses Leaflet, JavaScript geolocation API and MQTT over WebSockets protocol to transform a smartphone user using this application as an IoT sensor to visualize their location on a map. Users can enter an MQTT message broker host and port to connect to, and once connected, they can send a topic and message to listeners subscribed on the same topic. Users can also share their location and a random generated temperature value to listeners subscribed to topic engo_551/iffah_hamdan/my_temperature, and then display this information on the map.

The video demo for this project can be found [here](https://www.youtube.com/watch?v=XymryKKfXi4)

This website was built with HTML and Javascript. The following tools, libraries and plugins were used in development:
- **[Leaflet.js](https://github.com/Leaflet/Leaflet)** for creating the interactive map
- **[Eclipse Paho JavaScript client](https://github.com/eclipse/paho.mqtt.javascript)** to connect to an MQTT broker via WebSockets
- **[Bootstrap 5](https://github.com/twbs/bootstrap)** to create the grid layout of the HTML page and styles for user input

## Project Files
**index.html** - HTML file defining the layout of the site and functionality for user inputs

**map.js** - JS file for creating the map and displaying the location marker based on the received GeoJson message containing the user's location over topic engo_551/iffah_hamdan/my_temperature

**websocket.js** - JS file for handling user inputs and websocket functionality
