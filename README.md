<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
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
  position:relative;
}

/* SCALE */
.scale{
  transform: scale(3.6);
  image-rendering: pixelated;
}

/* IDLE */
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

.eye.blink{
  animation: blink 4s infinite;
}
@keyframes blink{
  0%,90%,100%{opacity:1;}
  93%{opacity:0;}
}

.jacket{background:#e8dfcf;}
.shirt{background:#ffffff;}
.pants{background:#1e1e1e;}
.shoe{background:#ffffff;}
.clear{clear:both;}

/* LAPTOP */
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
