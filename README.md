# S3

It's very easy to make some words **bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com)



# This is an h1 tag
## This is an h2 tag
###### This is an h6 tag

* Item 1
* Item 2
  * Item 2a
  * Item 2b
  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

<img src="Logo_AsTICo.png" style="float:center" width="30%">

http://github.com - automatic!
[GitHub](http://github.com)

As Kanye West said:
> We're living the future so
> the present is our past.

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content1 in the first column | :
Content2 in the first column | Content2 in the second column
Content3 in the first column | Content3 in the second column

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
