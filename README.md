# ACC_Telemetry
This is code that will show data from the game Assetto Corsa Competizione. Things like lap time, sector time, gear shifts, and temperatures will be shown to help produce faster lap times.

# How to make this code work:
    - Install all of the dependencies and export your telemetry folder
    - Then run main.py, all of the .py documents work together in this one document.
    - The idparser file will parse MoTeC data so that you can see it in this code.
    

### Dependencies to install
    pip3 install -r requirements.txt

### Usage
    export TELEMETRY_FOLDER=='/../Documents/Assetto Corsa Competizione/MoTeC'
    bokeh serve --show .

### Docker Image
    docker build -t acctelemetry .
    docker run --name acctelemetry -p 5100:5100 -e ORIGIN=www.example.com:5100 -d --rm acctelemetry
