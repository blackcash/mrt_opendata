# Open data 捷運站坐標
============
### 做法
- 透過捷運站的[官方網站](http://web.trtc.com.tw/c/stationdetail2010.asp?ID=19)來取得
再 ruby gem `"geocoder"` 透過地址來取得經緯度，example: "10576臺北市松山區敦化北路338號" -> "25.063718, 121.549643"

### 捷運站坐標: `mrt.json`

```
[
  {
    "id": 1,
    "name": "松山機場",
    "number": "7",
    "address": "10576臺北市松山區敦化北路338號",
    "latitude": 25.063718,
    "longitude": 121.549643
  },
  {
    "id": 2,
    "name": "中山國中",
    "number": "8",
    "address": "10476臺北市中山區復興北路376號",
    "latitude": 25.0607843,
    "longitude": 121.5439248
  },
  ...
```

### reference
- [www.trtc.com.tw](http://www.trtc.com.tw/ct.asp?CtNode=24569&mp=122031&xItem=1015926)
- ruby gem [geocoder](http://www.rubygeocoder.com/)