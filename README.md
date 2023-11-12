# ACC_Telemetry
This is code that will show data from the game Assetto Corsa Competizione. Things like lap time, sector time, gear shifts, and temperatures will be shown to help produce faster lap times.

### Dependencies to install
    pip3 install -r requirements.txt

### Usage
    export TELEMETRY_FOLDER=='/../Documents/Assetto Corsa Competizione/MoTeC'
    bokeh serve --show .

### Docker Image
    docker build -t acctelemetry .
    docker run --name acctelemetry -p 5100:5100 -e ORIGIN=www.example.com:5100 -d --rm acctelemetry
