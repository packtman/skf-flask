![Alt text](http://www.securityknowledgeframework.com/img/profile.png)

#Security Knowledge Framework
Security Knowledge Framework is an expert system application that uses OWASP Application Security Verification Standard, code examples, helps developers in pre-development and post-development.

##Table of Contents
* [Introduction](#introduction)
* [Installing](#installing)
* [Usage](#usage)
* [Testing](#testing)
* [License](#license)
* [Contributors](#contributors)

##<a name="introduction"></a>Introduction
Our experience taught us that the current level of security the current web-applications contain is not sufficient enough to ensure security. This is mainly because web-developers simply aren't aware of the risks and dangers which are lurking, waiting to be exploited by hackers.

Because of this we decided to develop a proof of concept framework in order to create a guide system available for all developers so they can develop applications secure by design.

The security knowledge framework is here to support developers create secure applications. By analysing processing techniques in which the developers use to edit their data the application can link these techniques to different known vulnerabilities and give the developer feedback regarding descriptions and solutions on how to properly implement these techniques in a safe manner.

The second stage of the application is validating if the developer properly implemented different types of defence mechanisms by means of checklists with among others the OWASP Application security verification standards.

By means of the answers supplied by the developer the application again generates documentation in which it gives feedback on what defence mechanisms the developer forgot to implement and give him feedback regarding descriptions and solutions on how to properly implement these techniques in a safe manner.

##<a name="installing"></a>Installing

####Ubuntu
----------
To run SKF you need Python pip and sqlite3 database support.
```bash
  sudo apt-get install python-pip sqlite3
```

After the prerequisites you can install the Python packages.
```bash
  pip install https://github.com/mitsuhiko/flask/tarball/master
  pip install owasp-skf
```

Now you can start the program by opening the folder (e.g. /opt/owasp-skf/) and run:
```bash
  python skf.py
```

####Windows
-----------
Download and install [Python 2.7.9](https://www.python.org/downloads/release/python-279/)

Run below commands in cmd:
```
  C:\Python27\Scripts\pip.exe install https://github.com/mitsuhiko/flask/tarball/master
  C:\Python27\Scripts\pip.exe install owasp-skf
```

Now you can start the program by opening the folder and run the skf.py file:
```
  cd C:\Python27\Lib\site-packages\skf
  C:\Python27\python.exe skf.py
```

##<a name="usage"></a>Usage

The application will greet you on `https://127.0.0.1:5443/`

Default the application will generate a certificate on the fly but what you really want to do is placing your own server.key and server.crt in the skf dir. Then the skf-flask application will use these instead.

Default username: `admin`
The password will be auto-generated every time the skf-application is launched. Check commandline output for the generated password.

##<a name="testing"></a>Testing
####Ubuntu:
-----------
```
  pip install pytest
```
####Windows:
------------
```
  C:\Python27\Scripts\pip.exe --install pytest
```

##<a name="license"></a>License
    Copyright (C) 2015  Glenn ten Cate, Riccardo ten Cate

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.

    You should have received a copy of the GNU Affero General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

####SKF includes the following software:
----------------------------------------
* [Certified secure](https://www.certifiedsecure.com/frontpage)  
Licensed under the [creative commons](http://creativecommons.org/licenses/by-nd/3.0/nl/) license

* [Owasp](http://owasp.com/index.php/Main_Page)  
Licensed under the [creative commons](http://creativecommons.org/licenses/by-nd/3.0/nl/) license

* [TCPDF](http://www.tcpdf.org/)  
Licensed under [GNU Lesser General Public](http://www.tecnick.com/pagefiles/tcpdf/LICENSE.TXT) License

* [jQuery](http://jquery.org)  
Licensed under the [MIT license](http://jquery.org/license)

* Boostrap theme thanks to http://www.blacktie.com

##<a name="contributors"></a>Contributors
- Clenn ten Cate
- Riccardo ten Cate
- Daniel Paulus <d.paulus@gmail.com>