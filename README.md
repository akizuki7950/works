<!DOCTYPE html>
<html>
<head>
  <script>
    function startTime(){
      var today = new Date();
      var hh = today.getHours();
      var mm = today.getMinutes();
      var ss = today.getSeconds();
      mm = checkTime(mm);
      ss = checkTime(ss);
      document.getElementById('clock').innerHTML = hh + ":" + mm + ":" + ss;
      var timeoutId = setTimeout(startTime, 500);
    }

    function checkTime(i){
      if(i < 10) {
        i = "0" + i;
      }
      return i;
    }
  
  </script>
<title>何品樺's page</title>
<style>
body {
  background-color: black;
  text-align: center;
  color: white;
  font-family: Arial, Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>About me</h1>
<img src="avatar.jpg" alt="Avatar" style="width:200px">
<p>清華大學資訊工程學系</p>
<p>基隆高中</p>

<hr size="2" align="center" noshade width="90%" color="0000ff">
<h2>Interests</h2>
<p>繪畫</p>
<p>烹飪</p>
<hr size="2" align="center" noshade width="90%" color="0000ff">
<h3>1111</h3>
<p>1. aaa</p>
<p>2. bbb</p>
<p>3. ccc</p>
<hr size="2" align="center" noshade width="90%" color="0000ff">

<p><a href="https://www.facebook.com/weisson.ho">Facebook</a><p>

<p><b><marquee>AAAAAAAAAAAAAAAAAAAAAAA</marquee></b></p>
<body onload="startTime()">
    簡單的時鐘
    <div id="clock"></div>
  </body>

</body>
</html>
