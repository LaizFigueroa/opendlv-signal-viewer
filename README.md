## OpenDLV Microservice to view signals in your web-browser

This repository provides source code to view any signals that are exchanged in a
running session using OpenDLV software ecosystem.

[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)

## Table of Contents
* [Dependencies](#dependencies)
* [Usage](#usage)
* [License](#license)


## Dependencies
No dependencies! The following dependencies are part of the source distribution:

* [bootstrap.css 4.0.0](https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css)
* [bootstrap 4.0.0](https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js)
* [Chart 2.7.1](https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.7.1/Chart.js)
* [jQuery 3.2.1](https://code.jquery.com/jquery-3.2.1.slim.min.js)
* [moment 2.20.1](moment-with-locales.min.js)
* [popper 1.12.9](https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js)
* [libcluon.js 0.0.51](https://github.com/chrberger/libcluon) - [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)


## Usage
This microservice is created automatically on changes to this repository via
Docker's public registry for:
* [x86_64](https://hub.docker.com/r/laiz/webview_ubuntu/)
* [armhf](https://hub.docker.com/r/laiz/webview/)

To use this microservice for viewing any messages from the OpenDLV Standard
Message Set that are exchanged in a running OpenDLV.io session running at
240, simply run it as follows:

```
docker run --rm -ti --net=host -p 8082:8082 laiz/webview --cid=240
```

Now, simply point your web-browser to the IP address and port 8082 where you
started this microservice to see any currently exchanged messages:

![screenshot from signal viewer](https://raw.githubusercontent.com/chalmers-revere/opendlv-signal-viewer/master/signal-viewer.gif)


## License

* This project is released under the terms of the BSD-3-Clause License

