# Abrevio Command Line Interface
This is the command line shell script for Abrevio services.
For more information please refer to [http://abrev.io](http://abrev.io).

## Prerequisites ##
The following programs should be installed before using Abrevio CLI:

- cURL visit http://curl.haxx.se/download.html to download it manually or use the package manager of your preference.

## Installation ##
Please follow these steps in order to install:

1. Clone this repository or download the ZIP file.
2. Copy the abrevio file to any place defined in the PATH environment variable.

## Usage ##
The Abrevio CLI is used to convert URLs in Abrevio words from the command line and to convert Abrevio words in URLs again.
The syntax to use the tool is the following:

- abrevio {-dhls} words/url

The parameters in brackets are optional and are used as follows:

- d Display only: This parameter is used to show the result in the command line. If it is not specified the script will try to call the default browser to open the link. 
- h Help: This parameter shows the usage information.
- l Language: Set the preferred language, three languages are valid (en, es, pt).
- s Simple: Only display the result.

## Examples ##
The following examples will show how this Abrevio CLI can be used:

Generating Abrevio words for Google:
```sh
$ abrevio http://www.google.com
house
```

Returning the URL in the standard output using the generated words:
```sh
$ abrevio -d house
http://www.google.com
```
