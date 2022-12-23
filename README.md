# Tang_Team_Repository
A repository for the WaterTalk Clinic 

Example usage of ThingSpeak's Python library:

    import thingspeak
    channel_id = <insert channel id here>
    write_api_key = '<insert write key here>'
    read_api_key = '<insert read key here>'
    if __name__ == "__main__":
        wr_channel = thingspeak.Channel(id=channel_id, api_key=write_api_key)
        wr_channel.update({'field1':88, 'field2':59, 'field3':17})
