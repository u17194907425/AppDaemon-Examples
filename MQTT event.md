```python
  self.listen_event(self.mqtt_test, "MQTT_MESSAGE", namespace="mqtt", topic="zigbee2mqtt/socket_3")
      
  # event_name - <class 'str'>
  # data - <class 'dict'> 
  # {
  #   'payload': '{"battery":100,"voltage":3045,"linkquality":57}',
  #   'topic': 'zigbee2mqtt/0x00158d0001e8802d'
  # }
  def mqtt_test(self, event_name, data, *args, **kwargs):
    self.log("__function__", 'INFO')
    self.log("__function__: %s " % type(event_name), 'INFO')
    self.log("__function__: %s " % pformat(event_name), 'INFO')
    self.log("__function__: %s " % type(data), 'INFO')
    self.log("__function__: %s " % pformat(data), 'INFO')
```
