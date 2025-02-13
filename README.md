<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kiss Day By MOMO</title>

    <style>
        body{
  background-color:#78e08f;
  margin:0;
}

.container{
  margin: auto;
  position: absolute;
  top: 50%; left: 50%;
  -webkit-transform: translate(-50%,-50%);
      -ms-transform: translate(-50%,-50%);
          transform: translate(-50%,-50%);
  width:232px;
}

.face{
  width:70px;
  height:30px;
  position:absolute;
  right:0;
  top:30px;
  border-top-right-radius:15px;
}

#r-ball{
  animation: kiss 4s ease infinite;
  background-color:white;
}

@keyframes kiss{
  40%{transform:translate(0px);}
  50%{transform:translate(30px) rotate(20deg);}
  60%{transform:translate(-33px);}
  67%{transform:translate(-33px);}
  77%{transform:translate(0px);}
}

.kiss{
  background-colo:red;
  width:13px;
  height:10px;
  background-color:white;
  border-radius:50%;
  border-left:5px solid;
}

.kiss-m{
  position:absolute;
  left:20px;
  top:22px;
  opacity:0;
  animation:kiss-m 4s ease infinite;
}

@keyframes kiss-m{
  0%{opacity:0;}
  55%{opacity:0;}
  55.1%{opacity:1;}
  66%{opacity:1;}
  66.1%{opacity:0;}
}

.mouth-r{
  animation:mouth-m 4s ease infinite;
}

@keyframes mouth-m{
  0%{opacity:1;}
  54.9%{opacity:1;}
  55%{opacity:0;}
  66%{opacity:0;}
  66.1%{opacity:1;}
}

.face:after{
  position:absolute;
  content:"";
  width:18px;
  height:8px;
  background-color:#badc58;
  left:-5px;
  top:20px;
  border-radius:50%;
}

.face:before{
  position:absolute;
  content:"";
  width:18px;
  height:8px;
  background-color:#badc58;
  right:-8px;
  top:20px;
  border-radius:50%;
  z-index:-1;
}

.face-r{
  left:0;
  top:37px;
}

.face-r:after{
  width:10px;
  height:10px;
  left:5px;
}

.face-r:before{
  width:10px;
  height:10px;
  right:-4px;
}
.eye{
  width:15px;
  height:14px;
  border-radius:50%;
  border-bottom:5px solid;
  position:absolute;
}

.eye-r-p{
  border-top:5px solid;
  border-bottom:0px solid;
}

.eye-l{
  left:10px;
}

.eye-r{
  right:5px;
}

.mouth{
  width:30px;
  height:14px;
  border-radius:50%;
  border-bottom:5px solid;
  position:absolute;
  bottom:-5px;
  transform:translate(3px);
  left:0;
  right:0;
  margin: auto;
}

.ball{
  border: 8px solid;
  width:100px;
  height:100px;
  border-radius:50%;
  display:inline-block;
  vertical-align:top;
  position:relative;
}

#r-ball{
  position:relative;
  z-index:40;
}


#l-ball{
  animation: close 4s ease infinite;
  position:relative;
  z-index:50;
  background-color:#fff;
}

.face-l{
  animation: face 4s ease infinite;
}

@keyframes close{
  0%{transform:translate(0)}
  20%{transform:translate(20px)}
  35%{transform:translate(20px)}
  55%{transform:translate(0px)}
  100%{transform:translate(0px)}
}

@keyframes face{
  0%{transform:translate(0) rotate(0);}
  10%{transform:translate(0) rotate(0);}
  20%{transform:translate(5px) rotate(-2deg);}
  28%{transform:translate(0) rotate(0);}
  35%{transform:translate(5px) rotate(-2deg);}
  50%{transform:translate(0) rotate(0);}
  100%{transform:translate(0) rotate(0);}
}

/* Left Ball (Bagni/Magenta) */
#l-ball {
  background-color: magenta;
}

/* Right Ball (Red to Pink Gradient) */
#r-ball {
  background: linear-gradient(to bottom, red, pink);
}

/* Glowing Gradient Text */
h1 {
  font-size: 40px;
  font-weight: bold;
  text-align: center;
  background: linear-gradient(45deg, #ff0000, #ff7300, #ff00ff, #ff1493);
  background-size: 400% 400%;
  -webkit-background-clip: text;
  color: transparent;
  animation: glowText 3s infinite linear;
  text-shadow: 0 0 10px rgba(255, 0, 0, 0.6), 
               0 0 20px rgba(255, 105, 180, 0.8), 
               0 0 30px rgba(255, 20, 147, 1);
}

@keyframes glowText {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* Container for Button */
.button-container {
  text-align: center;
  margin-top: 20px; /* Space below the balls */
}

/* Stylish Glowing Button */
.button {
  display: inline-block;
  padding: 15px 30px;
  font-size: 20px;
  font-weight: bold;
  color: white;
  text-transform: uppercase;
  background: linear-gradient(45deg, #ff0000, #ff7300, #ff00ff, #ff1493);
  border: none;
  border-radius: 30px;
  cursor: pointer;
  box-shadow: 0 0 10px rgba(255, 0, 0, 0.8), 
              0 0 20px rgba(255, 105, 180, 0.8), 
              0 0 30px rgba(255, 20, 147, 1);
  animation: glowButton 3s infinite linear;
  transition: 0.3s;
}

.button:hover {
  transform: scale(1.1);
}

@keyframes glowButton {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}


/* Import Cool Font */
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

/* Stylish Glowing Text */
h1 {
  font-size: 40px;
  font-weight: bold;
  text-align: center;
  font-family: 'Pacifico', cursive; /* Stylish Font */
  background: linear-gradient(45deg, #ff0000, #ff7300, #ff00ff, #ff1493);
  background-size: 400% 400%;
  -webkit-background-clip: text;
  color: transparent;
  animation: glowText 3s infinite linear;
  text-shadow: 0 0 10px rgba(255, 0, 0, 0.6), 
               0 0 20px rgba(255, 105, 180, 0.8), 
               0 0 30px rgba(255, 20, 147, 1);
}

@keyframes glowText {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}



/* Button at the Bottom */
.button-container {
  position: absolute;
  bottom: 20px; /* Adjust as needed */
  width: 100%;
  text-align: center;
}

      </style>

</head>
<body>
    <h1>Happy Kiss Day</h1>

    <div class='container'>
        <div id='l-ball' class='ball'>
          <div class='face face-l'>
            <div class='eye eye-l'></div>
            <div class='eye eye-r'></div>
            <div class='mouth'></div>
          </div>
        </div><div id='r-ball' class='ball'>
          <div class='face face-r'>
            <div class='eye eye-l eye-r-p'></div>
            <div class='eye eye-r eye-r-p'></div>
            <div class='mouth mouth-r'></div>
            <div class='kiss-m'>
         
              <div class='kiss'></div>
              <div class='kiss'></div>
            </div>
          </div>
        </div>
      </div>


<!-- Button Below the Balls -->
<div class="button-container">
    <button class="button" onclick="window.location.href='main.html'">Click Me</button>
  </div>
      
</body>
</html>
