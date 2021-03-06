# Vaccine Notifier with Crontab
It takes input as music/song file path and other filter option for vaccine slot booking (given in usage section), Notifies you when vaccine slots are open for booking by sending desktop notification with song/music playing. 

## Installation

### From PyPI
```pip install vaccine-notifier```


### From GitHub
```
git clone https://github.com/panchal999/vaccine-notifier
python3 -m venv testenv
source testenv/bin/activate
python setup.py install
```

## Features
- Play Music/Song when vaccine slot detected
- Send customized desktop notification includes Pincode, Address and Date for available vaccine centers
- More details about Vaccine Centers updated in log file 

## Usage
### CLI
```
❯ vaccine-notifier -h
usage: vaccine-notifier [-h] [-p PINCODES] [-d DATES] [-v VACCINE] [-l LOG]
                        music

positional arguments:
  music                 Path of Music or Song file. Play when vaccination
                        center detected

optional arguments:
  -h, --help            show this help message and exit
  -p PINCODES, --pincodes PINCODES
                        Single Pincode OR Comma Sprated Pincodes if multiple
  -d DATES, --dates DATES
                        Single Date OR Comma Seprated dates if multiple (In
                        dd-mm-yyyy)
  -v VACCINE, --vaccine VACCINE
                        Vaccine Names, Comma Seprated if multiple FROM
                        (covishild, covaxin, sputnik)
  -l LOG, --log LOG     Log File to Store Logs (Default vaccine_log.log file in
                        current directory
```

## License

© 2020 Parth Panchal

This repository is licensed under the MIT license. See LICENSE for details.