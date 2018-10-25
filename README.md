# node-webcam-server

a simple node.js webcam server based on the livecam npm module

### Prerequisites

- A Webcam
- Node.js & [Yarn](https://yarnpkg.com/en/) or NPM
- GStreamer 1.3+ runtime

### Install

Follow the instructions to set up gstreamer detailed here on the [livecam readme](https://github.com/sepehr-laal/livecam/blob/master/README.md)

Clone the repo

```
git clone https://github.com/fmacpro/node-webcam-server.git
```

install dependencies

```
yarn install
```

### Running the cam server

you can run the app by simply doing the following command from the repo root

```
node webcam.js
```

this will serve a UI on port 11000 (http://localhost:11000) for debugging as well as a socket.io socket on port 12000 which broadcasts GStreamer's video frames for consumption on the browser side. See [livecam readme](https://github.com/sepehr-laal/livecam/blob/master/README.md) for more details.

### Setting the right Webcam if there are more than one like on a laptop for example

note: this script has only been tested on raspbian linux

run the bash script called cam.sh - this will set the last connected webcam as the first camera (which will be used by the script).

```
chmod +x cam.sh
```

```
./cam.sh
```

## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE Version 3 - see the [LICENSE.md](LICENSE.md) file for details
