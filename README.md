<!DOCTYPE html>
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
  height:100 vh;
  gap:140 px;
  overflow:hidden;
}

/* SCALE */
.scale{
  transform: scale (3.6);
  image-rendering: pixelated;
  position:relative;
}

/* PIXEL */
.pixel{
  width:5 px;
  height:5 px;
  float:left;
}
.clear{clear:both;}

/* COLORS */
.bg{background:transparent;}
.out{background:#111;}
.hair{background:#2a2a2a;}
.skin{background:#f4cfbb;}
.eye{background:#2b2b2b;}
.jacket{background:#e8dfcf;}
.shirt{background:#ffffff;}
.pants{background:#1e1e1e;}
.shoe{background:#ffffff;}

.eye.blink{animation:blink 4 s infinite;}
@ keyframes blink{
  0% ,90% ,100%{opacity:1;}
  93%{opacity:0;}
}

/* CHARACTER */
.chibi{animation:breathe 2.5 s ease-in-out infinite;}
@keyframes breathe{
  0%,100%{transform:translate Y (0);}
  50%{transform:translate Y (-3 px);}
}

/* LAPTOP */
.laptop{animation:typing 1.2 s infinite;}
@keyframes typing{
  0%,100%{transform:translate Y (0);}
  50%{transform:translate Y (1 px);}
}
.frame{background:#111;}
.screen{background:#3cff7a;}
.keyboard{background:#999;animation:keys .4s infinite alternate;}
@keyframes keys { 
  from {filter:brightness (1);}
  to {filter:brightness (1.4);}
}

/* SHARK */
.shark{
  position:absolute;
  left:-90 px;
  top:45 px;
  animation:sharkFloat 2.2 s ease-in-out infinite;
}
@keyframes sharkFloat{
  0%,100%{transform:translate Y (0);}
  50%{transform:translate Y (-4 px);}
}
.shark-body{background:#8fd3ff;}
.shark-eye{background:#000;}
.shark-mouth{background:#ff6b6b;}

/* BUBBLES */
.bubbles{
  position:absolute;
  inset:0;
  pointer-events:none;
}
.bubble{
  position:absolute;
  width:22 px;
  height:22 px;
  background:#ffffff55;
  border:2 px solid #ffffffaa;
  image-rendering:pixelated;
  animation:rise 3.5 s linear infinite;
}
@keyframes rise{
  0%{transform:translate Y (0);opacity:0;}
  10%{opacity:1;}
  100%{transform:translate Y (-180 px);opacity:0;}
}
</style>
</head>

<body>

<!-- BUBBLES -->
<div class="bubbles">
  <div class="bubble" style="left:10%; bottom:-30 px;"></div>
  <div class="bubble" style="left:25%; bottom:-40 px; animation-delay:1s;"></div>
  <div class="bubble" style="left:40%; bottom:-35 px; animation-delay:2s;"></div>
  <div class="bubble" style="left:60%; bottom:-45 px; animation-delay:.5s;"></div>
  <div class="bubble" style="left:80%; bottom:-30 px; animation-delay:1.5s;"></div>
</div>

<!-- CHARACTER + SHARK -->
<div class="scale">

  <!-- SHARK -->
  <div class="shark">
    <div class="pixel bg"></div><div class="pixel shark-body"></div><div class="pixel shark-body"></div><div class="pixel shark-body"></div><div class="pixel bg"></div><div class="clear"></div>
    <div class="pixel shark-body"></div><div class="pixel shark-body"></div><div class="pixel shark-eye"></div><div class="pixel shark-body"></div><div class="pixel shark-body"></div><div class="clear"></div>
    <div class="pixel shark-body"></div><div class="pixel shark-mouth"></div><div class="pixel shark-body"></div><div class="pixel shark-body"></div><div class="pixel bg"></div><div class="clear"></div>
  </div>

  <!-- CHIBI (TALL) -->
  <div class="chibi">

    <!-- HEAD -->
    <div class="pixel bg"></div><div class="pixel out"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel out"></div><div class="pixel bg"></div><div class="clear"></div>
    <div class="pixel out"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel hair"></div><div class="pixel out"></div><div class="clear"></div>
    <div class="pixel out"></div><div class="pixel hair"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel hair"></div><div class="pixel out"></div><div class="clear"></div>

    <!-- FACE -->
    <div class="pixel out"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel eye blink"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel eye blink"></div><div class="pixel skin"></div><div class="pixel out"></div><div class="clear"></div>
    <div class="pixel out"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel skin"></div><div class="pixel out"></div><div class="clear"></div>

    <!-- BODY (TALL) -->
    <div class="pixel bg"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel shirt"></div><div class="pixel shirt"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>
    <div class="pixel bg"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel jacket"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>

    <!-- LEGS -->
    <div class="pixel bg"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>
    <div class="pixel bg"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel pants"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="pixel bg"></div><div class="clear"></div>

    <!-- SHOES -->
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
