```python
import appdaemon.plugins.hass.hassapi as hass
#import glob
#import json
#from pprint import pformat

class NAME(hass.Hass):

  PARAM = ''

  def initialize(self):
    self.log("__function__", 'INFO')
    #code here
    # self.log("__function__: %s " % type(var), 'INFO')
    # self.log("__function__: var (%s) " % pformat(var), 'INFO')
    
    self.PARAM = self.args["PARAM"]

    self.listen_state(self.cb_state, "device_tracker.my_phone")




  def cb_state(self, entity, attribute, old, new, kwargs):
    self.log("__function__", 'INFO')
    #code here



```
