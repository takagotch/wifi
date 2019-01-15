### wifi
---
https://github.com/rockymeza/wifi

```
pip install wifi
WIFI_CLI_NAME=cool-wifi pip install wifi
WIFI_INSTALL_CLI=False pip install wifi
python -m wifi

wifi scan
wifi scan | sort -rn
wifi connect --ad-hoc SomeNet
wifi add some SomeNet
wifi connect some
wifi list

```

```
from wifi import Cell, Scheme
Cell.all('wlan0')

cell = Cell.all('wlan0')[0]
scheme = Scheme.for_cell('wlan0', 'home', cell, passkey)
scheme.save()
scheme.activate()

scheme = Scheme.find('wlan0', 'home')
scheme.activate()
```

```
```


