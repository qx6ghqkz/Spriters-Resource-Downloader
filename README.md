[![GitHub license](https://img.shields.io/github/license/qx6ghqkz/Spriters-Resource-Downloader.svg)](https://github.com/qx6ghqkz/Spriters-Resource-Downloader/blob/main/LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/qx6ghqkz/Spriters-Resource-Downloader/pulls)
[![GitHub contributors](https://img.shields.io/github/contributors/qx6ghqkz/Spriters-Resource-Downloader.svg)](https://github.com/qx6ghqkz/Spriters-Resource-Downloader/graphs/contributors)
[![GitHub issues](https://img.shields.io/github/issues/qx6ghqkz/Spriters-Resource-Downloader.svg)](https://github.com/qx6ghqkz/Spriters-Resource-Downloader/issues)

<p align="center">
  <h1 align="center">Spriters Resource Downloader</h3>

  <p align="center">
    A downloader for the website <a href="https://www.spriters-resource.com">Spriters Resource</a>
    <br />
    <a href="https://github.com/qx6ghqkz/Spriters-Resource-Downloader/issues">Report a bug or request a feature</a>
  </p>
</p>

## Table of Contents

* [Introduction](#introduction)
* [Getting Started](#getting-started)
  * [Prerequisites and dependencies](#prerequisites-and-dependencies)
  * [Installation](#installation)
* [Usage](#usage)
  * [Command line options](#command-line-options)
* [Contributing](#contributing)
* [License](#license)

## Introduction

This repository contains a command line application to simply download all sprites and spritesheets of a given game from the website [Spriters Resource](https://www.spriters-resource.com) (`https://www.spriters-resource.com`).

## Getting Started

For users, you can just download the [latest release](https://github.com/qx6ghqkz/Spriters-Resource-Downloader/releases/latest) of the application and jump [here](#usage).

Next information is mainly dedicated to developers who wants to run the application in a more pythonish way.

### Prerequisites and dependencies

This repository is tested on Python 3.7+.

You should install Spriters Resource Downloader in a [virtual environment](https://docs.python.org/3/library/venv.html). If you're unfamiliar with Python virtual environments, check out the [user guide](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
First, create a virtual environment with the version of Python you're going to use and activate it.

You can install directly all required packages by using the file `requirements.txt` and doing:
```bash
pip install -r requirements.txt
```

### Installation

Follow the instructions above then clone the repo (`git clone https:://github.com/qx6ghqkz/Spriters-Resource-Downloader.git`).\
You can now launch the app by running `spriters-resource-downloader.py`.

## Usage

Just launch the application with:

For users:
```
spriters-resource-downloader.exe [-h] [-v] [--nsfw] url
```

For developers:
```
python spriters-resource-downloader.py [-h] [-v] [--nsfw] url
```

### Command line options

Here are the possible arguments:

```
positional arguments:
  url            URL to a game on the website spriters-resource.com

optional arguments:
  -h, --help     show this help message and exit
  -v, --verbose  use it to print progress during download
  --nsfw         use it to enable downloading of NSFW assets
```

It is recommended to activate the verbose mode (optional, not activated by default) to keep track of the progress.

### Example

The next command line will download all the sprites referenced on this [page](https://www.spriters-resource.com/game_boy_gbc/pokemongoldsilver/) and put them in the folder `downloaded/game_boy_gbc/pokemongoldsilver/` while printing progress during download:

For users:
```
spriters-resource-downloader.exe -v https://www.spriters-resource.com/game_boy_gbc/pokemongoldsilver/
```

For developers:
```
python spriters-resource-downloader.py -v https://www.spriters-resource.com/game_boy_gbc/pokemongoldsilver/
```


## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->
## License

Distributed under the GNU General Public License v3.0. See `LICENSE` for more information.
