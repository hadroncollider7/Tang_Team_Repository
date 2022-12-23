# Tang_Team_Repository
A repository for the WaterTalk Clinic 

Example usage of ThingSpeak's Python library:

import thingspeak
​
​
channel_id = 1966115
write_api_key = 'CB6PC3SMZRE3CMBH'
read_api_key = '0QQ9K865AMO5SJXJ'
​
if __name__ == "__main__":
    wr_channel = thingspeak.Channel(id=channel_id, api_key=write_api_key)
    wr_channel.update({'field1':88, 'field2':59, 'field3':17})
