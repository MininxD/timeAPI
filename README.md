# TimeAPI 
TimeAPI adalah Interface Program untuk waktu dan tanggal, dengan berbasis unix



[![GitHub tag](https://img.shields.io/github/tag/mininxd/timeAPI?include_prereleases=&sort=semver&color=blue)](https://github.com/mininxd/timeAPI/releases/)
[![License](https://img.shields.io/badge/License-MIT-blue)](https://github.com/mininxd/timeAPI/blob/main/LICENSE)
[![issues - timeAPI](https://img.shields.io/github/issues/mininxd/timeAPI)](https://github.com/mininxd/timeAPI/issues)
<br>
![maintained - yes](https://img.shields.io/badge/maintained-yes-blue)
[![endpoint - https://timeapi.mininxd.my.id/](https://img.shields.io/badge/endpoint-https%3A%2F%2Ftimeapi.mininxd.my.id%2F-2ea44f?logo=vercel)](https://timeapi.mininxd.my.id/)

<br>

***API Call:*** <br>
![Waktu Indonesia Barat](https://img.shields.io/badge/dynamic/json?label=Waktu+Indonesia+Barat&query=wib%5B0%5D.time24&url=https%3A%2F%2Ftimeapi.mininxd.my.id)
![Waktu Indonesia Tengah](https://img.shields.io/badge/dynamic/json?label=Waktu+Indonesia+Tengah&query=wita%5B0%5D.time24&url=https%3A%2F%2Ftimeapi.mininxd.my.id)
![Waktu Indonesia Timur](https://img.shields.io/badge/dynamic/json?label=Waktu+Indonesia+Timur&query=wit%5B0%5D.time24&url=https%3A%2F%2Ftimeapi.mininxd.my.id)
<br>

***Deploy TimeAPI pakai Vercel***<br>
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fmininxd%2FtimeAPI)


<br>

## Tutorial

### Cara mengubah TimeZone jika kamu deploy ke vercel

dalam file /api/index.js terdapat kode<br>
```javascript
var unixTime = Number(response.body) + Number(GMT0);
````
beserta 
```javascript
var unixWib = Number(response.body) + Number(GMT7);
var unixWita = Number(response.body) + Number(GMT8);
var unixWit = Number(response.body) + Number(GMT9);
```
<br>
kamu tinggal ubah "GMT"nya saja yang sudah disediakan dalam tz-data.js
<br>


Jika kamu mau pakai GMT lain yang tidak tertera pada tz-data, kamu bisa pakai converter UNIX
**[disini](https://mininxd.github.io/timeAPI/docs/)**
<br>
<br>
### bagaimana jika GMT/Zonawaktu itu GMT- (ada minusnya)?
Tinggal ubah kode 
```javascript
var unixTime = Number(response.body) + Number(GMT0);
```
menjadi pengurangan<br>
```javascript
var unixTime = Number(response.body) - Number(GMT0);
```

<br>

<center>
 
  [![Donate - Saweria](https://img.shields.io/badge/Donate-Saweria-2ea44f?style=for-the-badge)](https://saweria.co/mininxd)
  [![Paypal](https://img.shields.io/badge/Paypal-blue?style=for-the-badge&logo=paypal)](https://paypal.me/mininxd?country.x=ID&locale.x=en_US)
</center>

