# Interactive-Web-PAge
Choosing an image file to be uploaded in a web page

Implemented on CodePen:

Link to the CodePen File: https://codepen.io/akshara1610/pen/OJMwyLZ

Uses HTML,CSS, JavaScript:

//Code HTML:
<html>
  <script src=http://www.dukelearntoprogram.com/course1/common/js/image/SimpleImage.js>
</script>
<h1>Choose and Upload a Picture</h1>
<canvas id="can">
  
</canvas>
  
<p>
  Filename:
  <input type="file" multiple="false" accept="image/*" id="finput" onchange="upload()">
 
</p>
</html>


//Code CSS:
h1{
  font-family: times new roman;
  color: dimgray;
}
body{
  margin: 10px;
}
canvas
{
  height: 2000px;
  width: 2000px;
  border: 1px solid gray
}
input{
  font-family: times new roman;
  color: black;
  font-size: 14pt;
}

//Code JavaScript:
function upload(){
  var imagecanvas=document.getElementById("can");
  var fileinput=document.getElementById("finput")
  var newimg=new SimpleImage(fileinput);
  newimg.drawTo(imagecanvas);
}

