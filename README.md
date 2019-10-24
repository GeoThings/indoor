---
tag: geothings
---

# Indoor Drawing

## How to edit
### Editor
https://master.apis.dev.openstreetmap.org/edit?editor=id
### [example]()
![](https://i.imgur.com/PylQRbh.png)
[link](https://master.apis.dev.openstreetmap.org/edit#map=21/22.95894/120.32433)

### tag
- name: 
- area: yes
- indoor: area, arch, floor, steps, wall
- level: 1, 2, 3...
- base_height: (m)
- height: (m)
- color: blue, gray, green, orange, red, white, yellow

## How to get data
### get bbox
![](https://i.imgur.com/tibBeKC.png)
put marker on the left bottom and top right

![](https://i.imgur.com/WrKuadv.png)
click "zoom to here" or just press z

![](https://i.imgur.com/ORNibF5.png)
get latitude and logithude from browser URL bar
### get xml data
[https://master.apis.dev.openstreetmap.org/api/0.6/map?bbox=\[left\],\[bottom\],\[right\],\[top\]](https://master.apis.dev.openstreetmap.org/api/0.6/map?bbox=120.324051\,22.958072\,120.324781\,22.959010)
### transform to geojson
https://tyrasd.github.io/osmtogeojson/

## Q&A