# Tang_Team_Repository
A repository for the WaterTalk Clinic 

## ThingSpeak Library for Python
ThingSpeak provides a library for use with Python. To install the library, use:

    pip install thingspeak

For detailed instructions on using the ThingSpeak library, [click here](https://thingspeak.readthedocs.io/en/latest/install.html).

Example usage of ThingSpeak's Python library:

    import thingspeak
    channel_id = <insert channel id here>
    write_api_key = '<insert write key here>'
    read_api_key = '<insert read key here>'
    if __name__ == "__main__":
        wr_channel = thingspeak.Channel(id=channel_id, api_key=write_api_key)
        wr_channel.update({'field1':<insert value here>, 'field2':<insert value here>, 'field3':<insert value here>})

If your script is having trouble importing the ThingSpeak module, check default python version:

    python --version

If default Python is version 2, then the library is installed under version 2. If the compiler is under Python 3, then it will not see the library. To add 'python3' as the aternate for 'python' with priority '3', use:

    sudo update-alternatives --install $(which python) python $(readlink -f $(which python3)) 3

Then, install the ThingSpeak library again.
