```python
import appdaemon.plugins.hass.hassapi as hass
import glob
import json

from pprint import pformat

class NAME(hass.Hass):

  def initialize(self):
    self.log("__function__", 'INFO')
    #code here
    # self.log("__function__: %s " % type(var), 'INFO')
    # self.log("__function__: var (%s) " % pformat(var), 'INFO')
    
    
```
