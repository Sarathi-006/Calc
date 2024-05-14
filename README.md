# Ex.08 Design of a Standard Calculator
## Date:

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script type="text/javascript">
    function dis(x){
        document.getElementById("inbox").value+=x;
    }
    function clr(){
        document.getElementById("inbox").value='';
        document.getElementById("res").innerHTML='';
    }
    function del(){
        var a=document.getElementById("inbox").value;
        var l=a.substring(0,a.length-1);
        document.getElementById("inbox").value=l;

    } 
    function fun(){
        
       a=document.getElementById("inbox").value;
       
    document.getElementById("res").innerHTML=a;
var i;
var f='';
var c=0;
for(let i=0;i<a.length;i++){
     
if(a[i]=='+'|| a[i]=='-' || a[i]=='x' || a[i]=='/' || a[i]=='^'){
    if(c==1){
         c=0;
    if(op=='+'){
    var r=parseFloat(num1)+parseFloat(f);
    document.getElementById("inbox").value=r;
    f=r;
}
else if(op=='-'){
        var r=parseFloat(num1)-parseFloat(f);
        document.getElementById("inbox").value=r;
        f=r;
}  
else if(op=='x'){
    var r=parseFloat(num1)*parseFloat(f);
        document.getElementById("inbox").value=r;
        f=r;
}
else if(op=='/'){
    var r=parseFloat(num1)/parseFloat(f);
        document.getElementById("inbox").value=r;
        f=r;
}
else if(op=='^'){
    var r=Math.pow(parseFloat(num1),parseFloat(f));
        document.getElementById("inbox").value=r;
        f=r;
}
} 
    var op=a[i];
    var num1=f;
    f='';
    c++;
}
else{
   f+=a[i];
}

   }

   if(op=='+'){
    var r=parseFloat(num1)+parseFloat(f);
    document.getElementById("inbox").value=r;

   
}
else if(op=='-'){
        var r=parseFloat(num1)-parseFloat(f);
        document.getElementById("inbox").value=r;
       
}
else if(op=='x'){
    var r=parseFloat(num1)*parseFloat(f);
        document.getElementById("inbox").value=r;
}  
else if(op=='/'){
    var r=parseFloat(num1)/parseFloat(f);
        document.getElementById("inbox").value=r;
}
else if(op=='^'){
    var r=Math.pow(parseFloat(num1),parseFloat(f));
        document.getElementById("inbox").value=r;
}
}
    
    </script>

</head>
<style>
body{
background-color:lightblue;
}
.container{
 position:relative;
margin-top:30px;
margin-left:35px;
width:260px;
height:425px;
background-color:rgb(86, 83, 83);
}
button{
width:60px;
height:50px;
padding:20px 40px 20px 20px;
border-right: none;
font-size:20px;
text-align: center;
color:white;
background-color: black;
}
input{
width:253px;
height:170px;
font-size:30px;
background-color: rgb(29, 27, 27);
color:white;

}
input[type=text]{
top:50%;
}
.initial{
    position: absolute;
    top:5%;
    margin-left: 37%;

}
#num{
  margin-left:-10px;
}
#res{
    position: absolute;
    top:0%;
    height:50px;
    color:white;
    
font-size:30px;
}
#b10{
padding-right:106px;
background:linear-gradient(to right,rgb(255, 30, 30),rgb(154, 3, 3));
}
.box{
    position:absolute;
    top:25%;
margin-left:35%;
   height:500px;
   width:340px;
    background-color:rgb(255, 0, 119);
    background:linear-gradient(to right,rgb(0, 119, 255),rgb(2, 192, 230));
    border-radius: 25px;
}
</style>
</head>
<body>
    <div class="initial">
        <h2>SARATHI S Calculator</h2>
        <h2 id="num">212223040144</h2>
    </div>
    
<div class="box">
<div class="container">
    <p id="res"></p>
<input type="text" id="inbox"name="input"><br>

<button onclick="clr()"> AC</button>
<button onclick="del()">DE</button>
<button onclick="dis('^')">^</button>
<button onclick="dis('/')">/</button><br>
<button name="1" onclick="dis('1')">1</button>
<button onclick="dis('2')">2</button>
<button onclick="dis('3')">3</button>
<button onclick="dis('+')">+</button ><br>
<button onclick="dis('4')">4</button>
<button  onclick="dis('5')">5</button>
<button onclick="dis('6')">6</button>
<button onclick="dis('-')">-</button><br>
<button onclick="dis('7')">7</button>
<button onclick="dis('8')">8</button>
<button onclick="dis('9')">9</button>
<button onclick="dis('x')" >x</button><br>
<button  onclick="dis('.')">.</button>
<button onclick="dis('0')">0</button>
<button id="b10" onclick="fun()">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=</button><br>
</div>
</div>
</body>
</html>
```
## OUTPUT:
![Screenshot 2024-05-14 210520](https://github.com/Sarathi-006/Calc/assets/149349756/c5ac7780-a219-41ae-9e80-fbcc5d5232e2)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
