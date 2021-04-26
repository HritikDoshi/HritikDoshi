<!DOCTYPE html>
<html>
<head>
  <a href="https://youtu.be/7aobRPg7BXI" target="_blank" data-keyframers-credit style="color: #000"></a>
  <style>
    :root {
  --duration: 5s;
  --ease: cubic-bezier(.6, 0, .2, 1);
}


* {
  position: relative;
  box-sizing: border-box;
}

html, body {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
}

svg {
  // outline: 1px solid blue;
}

.digit {
  stroke-width: 30;
  animation: var(--duration) var(--ease) both alternate infinite;
  animation-delay: calc( (var(--i) * 0.05s));
  
  //animation-play-state: paused;
  
  circle,
  path {
    animation: inherit;
    stroke: var(--color);
    stroke-linejoin: round;
    stroke-linecap: round;
    /* Additional offsets for rounded stroke */
    stroke-dashoffset: -1.2;
    stroke-dasharray: 1 1.2;
  }
  
  circle {

    animation-name: circle-draw;
    
    @keyframes circle-draw {
      0%, 5% {  
        stroke-dasharray: 0 1.2 .2 .3;
        stroke-dashoffset: 1.75; 
      }

      18%, 50% {
        stroke-dasharray: 1 1.1;
        stroke-dashoffset: 0; 
      }
      70%, 100% { stroke-dashoffset: -1.1; }
    }
  }
  
  path {
    animation-name: path-draw;
    
    @keyframes path-draw {
      0%, 43% { stroke-dashoffset: 1.1; }
      //25%, 50% { stroke-dashoffset: 0; }
      90%, 100% { stroke-dashoffset: 0; }
    }
  }
}

.digit {
  
  animation-name: digit;
  
  &:nth-child(1) {
    --x-offset: 150%;
  }
  &:nth-child(2) {
    --x-offset: 50%;
  }
  &:nth-child(3) {
    --x-offset: -50%;
  }
  &:nth-child(4) {
    --x-offset: -150%;
  }
  
  &:nth-child(even) {
    // pixel pushing by Shaw™
    --y-offset: calc(-25% + 2%);
  }
  &:nth-child(odd) {
    --y-offset: calc(25% - 12%);
  }
  
  @keyframes digit {
    from, 15% {
      transform:
        translate(var(--x-offset, 0),var(--y-offset, 0));
    }
    30% {
      transform:
        translate(0%, var(--y-offset));
    }
    45%, to {
      transform: none;
    }
  }
}

.digits {
  display: flex;
  flex-direction: row;
}
  </style>
</head>
<body>
  <div class="digits">
  
  <svg class="digit" 
       viewBox="-20 -20 140 240" 
       width="100" 
       height="200" 
       stroke-width="20"
       fill="none"
       style="--color: #5288E1; --i: 1">

    <circle r="50" cx="50" cy="50" 
            pathLength="1" />

    <path
      pathLength="1"
      d="M0 50
         C 0 0, 50 0, 50 0
         C 100 0, 100 50, 100 50
         L 0 200
         L 100 200"
    />
  </svg>

  <svg class="digit" 

       viewBox="-20 -20 140 240" 
       width="100" 
       height="200" 
       stroke-width="20"
       fill="none"
       style="--color: #3DA658; --i: 2">

    <circle r="50" cx="50" cy="150" 
            stroke="#F00" 
            pathLength="1" />

    <path
      pathLength="1"
      d="M 100 150
         C 100 200, 50 200, 50 200
         C 0 200, 0 150, 0 150
         L 0 50
         C 0 0, 50 0, 50 0
         C 100 0, 100 50, 100 50
         L 100 150"
    />
  </svg>

  <svg class="digit" 
       viewBox="-20 -20 140 240" 
       width="100" 
       height="200" 
       stroke-width="20"
       fill="none"
       style="--color: #EFBE1B; --i: 3">

    <circle r="50" cx="50" cy="50" 
            pathLength="1" />

    <path
      pathLength="1"
      d="M0 50
         C 0 0, 50 0, 50 0
         C 100 0, 100 50, 100 50
         L 0 200
         L 100 200"
    />
  </svg>

  <svg class="digit" 
       viewBox="-20 -20 140 240" 
       width="100" 
       height="200" 
       stroke-width="20"
       fill="none"
       style="--color: #D7483D; --i: 4">

    <circle r="50" cx="50" cy="150" 
            pathLength="1" />

    <path
      pathLength="1"
      d="M 100 150
         C 100 200, 50 200, 50 200
         C 0 200, 0 150, 0 150
         L 0 50
         C 0 0, 50 0, 50 0
         C 100 0, 100 50, 100 50
         L 100 150"
    />
  </svg>
</div>

</body>
</html>




# Hi, !’m Hritik Doshi👋

- 📚 I'm a Electronics & Telecommunication Engineering student.
- 👀 I’m interested in Frontend Developing and working on Arduino projects.
- 🌱 I’m currently learning Python.
- 💞️ I’m looking to collaborate on Arduino or any other microcontroller Projects for building digital devices and also on Full stack projects.
- 🤗 I'm looking for help with Raspberry Pi and Python Projects.

  <link rel="stylesheet" href=("https://use.fontawesome.com/releases/v5.15.3/css/all.css") integrity=("sha384-SZXxX4whJ79/gErwcOYf+zWLeJdY/qpuqC4cAa9rOGUstPomtqpuNWT9wdPEn2fk") crossorigin="anonymous">
 
<!---
HritikDoshi/HritikDoshi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<p> <i class="fab fa-github" aria-hidden="true"></i> </p>


![Github stats](https://github-readme-stats.vercel.app/api?username=HritikDoshi)
