|                                                              | Tags für eine Fläche                                         | Tags für einen Way                                           |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![314_1040-32](img\314_1040-32.png)                          | `parking:condition=disc`<br />`maxstay=TIME`<br />           | `parking:condition:SEITE=disc`<br />`parking:condition:SEITE:maxstay=TIME`<br /> |
| ![314_1040-32_1042-33](img\314_1040-32_1042-33.png)          | `parking:condition=free`<br />`parking:condition:conditional=disc @ OPENING_HOURS`<br />`maxstay=no`<br />`maxstay:conditional=TIME @ (OPENING_HOURS)` | `parking:condition:SEITE:maxstay=no`<br />`parking:condition:SEITE:maxstay:conditional=TIME @ (OPENING_HOURS)`<br />`parking:condition:SEITE=free`<br />`parking:condition:SEITE:conditional=disc @ (OPENING_HOURS)` |
| ![314_1040-32_1042-33_1020-32](C:\Users\wiela\Documents\ownCloud\Documents\Dokumentation\OSM\parking\img\314_1040-32_1042-33_1020-32.png) | `parking:condition=residents`<br />`parking:condition:residents=AUSWEIS`<br />`parking:condition:conditional=disc @ OPENING_HOURS`<br />`maxstay=no`<br />`maxstay:conditional=TIME @ (OPENING_HOURS);no @ residents` | `parking:condition:SEITE=free`<br />`parking:condition:SEITE:residents=AUSWEIS`<br />`parking:condition:SEITE:conditional=disc @ OPENING_HOURS; free @ residents`<br />`parking:lane:SEITE:maxstay=no`<br />`parking:lane:SEITE:maxstay:conditional=TIME @ (OPENING_HOURS); no @ residents` |
| ![314_1040-32_1020-32](C:\Users\wiela\Documents\ownCloud\Documents\Dokumentation\OSM\parking\img\314_1040-32_1020-32.png) | `residents=AUSWEIS`<br />`parking:condition=disc`<br />`maxstay=TIME`<br />`maxstay:conditional=no @ residents`<br />`parking:condition:conditional= free @ residents` | `parking:condition:SEITE=disc`<br />`parking:condition:SEITE:residents=AUSWEIS`<br />`parking:condition:SEITE:conditional=free @ residents`<br />`parking:lane:SEITE:maxstay=TIME`<br />`parking:lane:SEITE:maxstay:conditional= no @ residents` |
| ![314_1044-10](img\314_1044-10.png)                          | `disabled=designated`                                        | `parking:conditional:SEITE:disabled=designated`              |
| ![314_1044-10_1042-33](img\314_1044-10_1042-33.png)          | `disabled=yes`<br />`disabled:conditional=designated @ (OPENING_HOURS)`<br />`vehicle=yes`<br />`vehicle:conditional=no @ (OPENING_HOURS)` | `parking:conditional:SEITE:disabled=yes`<br />`parking:conditional:SEITE:disabled:conditional=designated @ (OPENING_HOURS)`<br />`parking:conditional:SEITE:vehicle=yes`<br />`parking:conditional:SEITE:vehicle:conditional=no_parking @ (OPENING_HOURS)` |
| ![314_1044-11](img\314_1044-11.png)                          | `access=permit`<br />`permit=AUSWEIS`                        | `parking:SEITE:access=permit`<br />`permit=AUSWEIS`          |
| ![314_1044-30](img\314_1044-30.png)                          | `parking:condition:residents=AUSWEIS`<br />`access=residents` | `parking:condition:SEITE:residents=AUSWEIS`<br />`parking:condition:SEITE=residents` |
| ![314_1053-31](img\314_1053-31.png)                          | `parking:condition=ticket`<br />`fee=yes`                    | `parking:condition:SEITE=ticket`<br />`parking:SEITE:fee=yes` |
| ![314_1053-31_1020-32](img\314_1053-31_1020-32.png)          | `parking:condition=ticket`<br />`parking:condition:conditional=free @ residents`<br />`fee=yes`<br />`fee:conditional=no @ residents` | `parking:condition:SEITE=ticket`<br />`parking:condition:SEITE:conditional=free @ residents` |
| ![314_1042-33](img\314_1042-33.png)                          | `access=no`<br />`access:conditional=yes @ (OPENING_HOURS)`  | `parking:condition:SEITE:vehicle=no`<br />`parking:condition:SEITE:vehicle=yes @ (OPENING_HOURS)` |
| ![314_1010-58](img\314_1010-58.png)                          | `motorcar=designated`<br />`vehicle=no`                      | `parking:condition:SEITE:motorcar=free`<br />`parking:condition:SEITE:vehicle=no_parking` |
| ![314_1010-51](img\314_1010-51.png)                          | `hgv=designated`<br />`vehicle=no`                           | `parking:condition:SEITE:hgv=free`<br />`parking:condition:SEITE:vehicle=no` |
| ![314_1010-62](img\314_1010-62.png)                          | `motorcycle=designated`<br />`vehicle=no`                    | `parking:condition:SEITE:motorcycle=free`<br />`parking:condition:SEITE:vehicle=no_parking` |
| ![314_1010-57](C:\Users\wiela\Documents\ownCloud\Documents\Dokumentation\OSM\parking\img\314_1010-57.png) | `bus=designated`<br />`tourist_bus=designated`<br />`vehicle=no` | `parking:condition:SEITE:bus=free`<br />`parking:condition:SEITE:tourist_bus=free`<br />`parking:condition:SEITE:vehicle=no_parking` |
| ![314_1010-57_1042-33](img\314_1010-57_1042-33.png)          | `vehicle=yes`<br />`vehicle:conditional=no @ (OPENING_HOURS)`<br />`bus=yes`<br />`bus:conditional=designated @ (OPENING_HOURS)`<br />`tourist_bus=yes`<br />`tourist_bus:conditional=designated @ (OPENING_HOURS)` | `parking:condition:SEITE:vehicle=yes`<br />`parking:condition:SEITE:vehicle:conditional=no_parking @ (OPENING_HOURS)`<br />`parking:condition:SEITE:bus=yes`<br />`parking:condition:SEITE:bus:conditional=designated @ (OPENING_HOURS)`<br />`parking:condition:SEITE:tourist_bus=yes`<br />`parking:condition:SEITE:tourist_bus:conditional=designated @ (OPENING_HOURS)` |
| ![286_1010-62](img\286_1010-62.png)                          | _[Wird nur an Ways verwendet]_                               | `parking:condition:SEITE:motorcycle=no_parking`              |
| ![286_1010-51](img\286_1010-51.png)                          | _[Wird nur an Ways verwendet]_                               | `parking:condition:SEITE:hgv=no_parking`                     |
| ![286_1042-33](img\286_1042-33.png)                          | _[Wird nur an Ways verwendet]_                               | `parking:condition:SEITE:conditional=no_parking @ (OPENING_HOURS)`<br />`parking:lane:SEITE:conditional=no @ (OPENING_HOURS)`<br />`parking:condition:SEITE=free` |
| ![286_1020-32](img\286_1020-32.png)                          | _[Wird nur an Ways verwendet]_                               | `parking:condition:SEITE=no_parking`<br />`parking:condition:SEITE:conditional=free @ residents` |



##### Platzhalter für Werte

- `SEITE` - Die Seite(n) des Way, für die die condition gilt. right/left/both
- `OPENING_HOURS` - Platzhalter für Zeitspannen, zu denen Beschränkungen gelten
- `TIME` - Zeit, die auf dem Parkscheiben-Schild steht
- `AUSWEIS` - Nr. des Parkausweises, die auf dem Schild angegeben ist