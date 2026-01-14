<html lang="en">
<head>
<meta charset="UTF-8">
<title>Chibi Pixel – Typing Mode</title>

<style>
body{
  margin:0;
  background:#000;
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
  gap:140px;
  overflow:hidden;
}

/* BIGGER SCALE */
.scale{
  transform: scale(3.6);
  image-rendering: pixelated;
}

/* IDLE + TYPING */
.chibi{
  animation: breathe 2.5s ease-in-out infinite;
}
@keyframes breathe{
  0%,100%{transform:translateY(0);}
  50%{transform:translateY(-3px);}
}

/* PIXEL */
.pixel{
  width:5px;
  height:5px;
  float:left;
}

/* COLORS */
.bg{background:transparent;}
.out{background:#111;}
.hair{background:#2a2a2a;}
.skin{background:#f4cfbb;}
.eye{background:#2b2b2b;}
.eye.blink{animation: blink 4s infinite;}
@keyframes blink{
  0%,90%,100%{opacity:1;}
  93%{opacity:0;}
}

.jacket{background:#e8dfcf;}
.shirt{background:#ffffff;}
.pants{background:#1e1e1e;}
.shoe{background:#ffffff;}
.clear{clear:both;}

/* LAPTOP + TYPING */
.laptop{
  animation: typing 1.2s infinite;
}
@keyframes typing{
  0%,100%{transform:translateY(0);}
  50%{transform:translateY(1px);}
}

.keyboard{
  background:#999;
  animation: keys 0.4s infinite alternate;
}
@keyframes keys{
  from{filter:brightness(1);}
  to{filter:brightness(1.4);}
}

.screen{background:#3cff7a;}
.frame{background:#111;}

/* BUBBLES */
.bubbles{
  position:absolute;
  inset:0;
  pointer-events:none;
}

.bubble{
  position:absolute;
  width:22px;
  height:22px;
  background:#ffffff55;
  border:2px solid #ffffffaa;
  image-rendering: pixelated;
  animation: rise 3.5s linear infinite;
}

@keyframes rise{
  0%{
    transform:translateY(0);
    opacity:0;
  }
  10%{opacity:1;}
  100%{
    transform:translateY(-180px);
    opacity:0;
  }
}
</style>
</head>

<body>

<!-- FAST BIG BUBBLES -->
<div class="bubbles">
  <div class="bubble" style="left:10%; bottom:-30px; animation-delay:0s;"></div>
  <div class="bubble" style="left:25%; bottom:-40px; animation-delay:1s;"></div>
  <div class="bubble" style="left:40%; bottom:-35px; animation-delay:2s;"></div>
  <div class="bubble" style="left:60%; bottom:-50px; animation-delay:0.5s;"></div>
  <div class="bubble" style="left:75%; bottom:-30px; animation-delay:1.5s;"></div>
  <div class="bubble" style="left:90%; bottom:-45px; animation-delay:2.5s;"></div>
</div>

<!-- CHARACTER -->
<div class="scale">
<div class="chibi">

<!-- HEAD -->
<div class="pixel bg"></div><div class="pixel out"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel out"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel out"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel out"></div><div class="clear"></div>

<div class="pixel out"></div><div class="pixel hair"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel hair"></div><div class="pixel out"></div><div class="clear"></div>

<!-- FACE -->
<div class="pixel out"></div><div class="pixel skin"></div><div class="pixel skin"></div>
<div class="pixel eye blink"></div>
<div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div>
<div class="pixel skin"></div>
<div class="pixel eye blink"></div>
<div class="pixel skin"></div><div class="pixel out"></div><div class="clear"></div>

<div class="pixel out"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel out"></div><div class="clear"></div>

<!-- BODY -->
<div class="pixel bg"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel shirt"></div><div class="pixel shirt"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel bg"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel bg"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel bg"></div><div class="pixel shoe"></div><div class="pixel shoe"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel shoe"></div><div class="pixel shoe"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>

</div>
</div>

<!-- LAPTOP -->
<div class="scale">
<div class="laptop">

<div class="pixel bg"></div><div class="pixel frame"></div><div class="pixel frame"></div><div class="pixel frame"></div><div class="pixel frame"></div><div class="pixel frame"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel frame"></div><div class="pixel screen"></div><div class="pixel screen"></div><div class="pixel screen"></div><div class="pixel screen"></div><div class="pixel frame"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel frame"></div><div class="pixel screen"></div><div class="pixel screen"></div><div class="pixel screen"></div><div class="pixel screen"></div><div class="pixel frame"></div><div class="pixel bg"></div><div class="clear"></div>

<div class="pixel bg"></div><div class="pixel keyboard"></div><div class="pixel keyboard"></div><div class="pixel keyboard"></div><div class="pixel keyboard"></div><div class="pixel keyboard"></div><div class="pixel bg"></div><div class="clear"></div>

</div>
</div>

</body>
</html>
