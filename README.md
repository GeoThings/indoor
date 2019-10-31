---
tags: geothings
---

# **Indoor Drawing**

## How to edit
### Editor
https://master.apis.dev.openstreetmap.org/edit?editor=id
### [example](https://master.apis.dev.openstreetmap.org/edit#map=21/22.95894/120.32433)
![](https://i.imgur.com/PylQRbh.png)

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
1. put marker on the left bottom and top right
![](https://i.imgur.com/tibBeKC.png)

1. click "zoom to here" or just press z
![](https://i.imgur.com/WrKuadv.png)

1. get latitude and logithude from browser URL bar
![](https://i.imgur.com/ORNibF5.png)

### get xml data
[https://master.apis.dev.openstreetmap.org/api/0.6/map?bbox=\[left\],\[bottom\],\[right\],\[top\]](https://master.apis.dev.openstreetmap.org/api/0.6/map?bbox=120.324051\,22.958072\,120.324781\,22.959010)

###### tags: 輸入時不用\

### transform to geojson
https://tyrasd.github.io/osmtogeojson/
### modify format
https://jqplay.org/
```
.features = [.features[]|.properties=(.properties.tags | .height=(.height|strings|tonumber) | .base_height=(.base_height|strings|tonumber) | .level=(.level|strings|tonumber))]
```

## <i class="fa fa-edit fa-fw"></i>Q&A

## Task
### 繪製旅館
- 位置：　https://tainan.chamcham.com.tw/location/
- 室內配置：https://geobingan.info/report/1241185ac0d346c8a98f2f5166a45769

## 上傳至Github
1. Fork https://github.com/Geothings/indoor
2. git clone from `https://github.com/[Your Github account]/indoor`
3. Add geojson files into `./data`
4. push to fork
5. Make PR to https://github.com/Geothings/indoor
6. Improve this doc, **add details to steps above**