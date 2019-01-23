 
<h1 align="center">
 <strong>Samsung Gear S3 Project</strong>
</h1>
<p align="center">
  <a href="#Watch">Samsung Gear S3 Watch</a> |
  <a href="#Data">Data Structure</a>
  <br><br>
  <img src="Logo_AsTICo.png" width="20%">
</p>

<h1 id="Watch">Samsung Gear S3 Watch <a href="#"><img src="top.png" witdh="1%"></a></h1>

<img src="s3.jpeg" width="20%">

* Item 1
* Item 2
  * Item 2a
  * Item 2b

<h1 id="Data">Data Structure <a href="#"><img src="top.png" witdh="1%"></a></h1>

```
typedef struct {
  unsigned long long timestamp;
  struct {
      float x, y, z;
  } acceleration;
  struct {
      float x, y, z;
    struct {
        float x, y, z;
    } drift;
  } gyroscope;
} WatchData;
```
sizeof(WatchData) is 48 bytes (6 times 8) and it's mapping in memory is:

 <table>
  <tr>
    <th>4 bytes (32 bits)</th>
    <th>4 bytes (32 bits)</th>
  </tr>
  <tr>
    <td align="center" colspan="2"><strong>unsigned long long</strong> timestamp</td>
  </tr>
  <tr>
    <td><strong>float</strong> acceleration.x</td>
    <td><strong>float</strong> acceleration.y</td>
  </tr>
  <tr>
    <td><strong>float</strong> acceleration.z</td>
    <td><strong>float</strong> gyroscope.x</td>
  </tr>
   <tr>
    <td><strong>float</strong> gyroscope.y</td>
    <td><strong>float</strong> gyroscope.z</td>
  </tr>
   <tr>
    <td><strong>float</strong> gyroscope.drift.x</td>
    <td><strong>float</strong> gyroscope.drift.y</td>
  </tr>
   <tr>
    <td><strong>float</strong> gyroscope.drift.z</td>
    <td></td>
  </tr>
</table> 
