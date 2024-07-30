# Urban-Exploration<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Urban Exploration 🕸️</title>

    <style>
        
        h1 {
            text-align: center;
            text-decoration: underline;
            
        }
        h2 { 
            text-align: center;
            font-size: 20px;
        }

        body {
            background: linear-gradient(109.6deg, rgb(72, 200, 160) 11.2%, rgb(32, 40, 48) 91.3%);
            font-family:'Courier New', Courier, monospace;   
        }

        img {
            display:block;
            margin: 10px auto;
            border-radius: 10px;
        }

        footer {
            text-align: center;
            font-size: 16px;
        }

        .container {
            display:block;
            margin: 20px auto;
            max-width: 600px;
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            font-size: 18px;
        }

        .intro-picture {
            max-width: 100%;
        }

        .intro-picture:hover {
            filter: contrast(80%);
            transform: scale(1.15);
            transition: all 150ms ease-in-out;
        }

        .grid {
            display:grid;
            grid-template-columns: 1fr 1fr 1fr 1fr;
            grid-gap: 20px;
        }

        .grid img {
            width: 100%;
        }

        .grid img:hover {
            filter: contrast(80%);
            transform: scale(2);
            transition: all 150ms ease-in-out;
        }

        button {
            display: block;
            margin: 0 auto;
            border: 1px solid white;
            background: white;
            border-radius: 45px;
            font-size: 18px;
            padding: 10px;
            font-family: 'Courier New', Courier, monospace;
        }
        button:hover {
            background: rgba(255, 255, 255, 0.5);
            color: rgba(0, 0, 0, 0.5);
            cursor: pointer;
            border: 1px solid white; 
            transition: all 150ms ease-in-out;           
        }


        .theme-button { 
            font-size: 12px;
            background: rgba(255, 255, 255, 0.7);
            color: #2c2d34;
            font-family: 'Courier New', Courier, monospace;
        }

        .theme-button:hover {
            background: #0f0f0fd3;
            cursor: pointer;
            color: #fff;
            transition: all 150ms ease-in-out;
        }

        .dark {
        background: radial-gradient(circle at 24.1% 68.8%,
         rgb(50, 50, 50) 0%, 
         rgb(0, 0, 0) 99.4%);
          color: white;
        }

        .dark .container {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 1px solid black;
        }

        .dark .theme-button {
            background: rgba(255, 255, 255, 0.2);
            color: #fff;
            border-radius: 1px solid white;
        }

        .dark .theme-button:hover {
            background: rgba(255, 255, 255, 0.8);
            cursor: pointer;
            color: #000;
            transition: all 150ms ease-in-out;
        }

        .dark a {
            color: white;
        }

    </style>

</head>

<body>
    <button class="theme-button"> Change Theme </button>

    <div class="container">

        <h1> Urban Exploration </h1>
        <h2> You never know what you may discover🌿🕸️</h2>

     <a href="https://en.wikipedia.org/wiki/Urban_exploration" target="_blank">
         <img src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/136/200/original/HT_abandoned_places_movies_jef_140620_21x13_1600.jpg?1722294986" 
         alt="auditorium" class="intro-picture"/>
     </a> 
       <hr>
        <div class="grid">
            <img src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/136/028/original/izzy-edey-HWoIuyRtZQw-unsplash-scaled-e1623271404684.jpg?1722188004" 
             alt="windows" width="300"/>  
            <img src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/136/199/original/231020125557-01-abandoned-places-reclaimed-by-nature-top-restricted.jpg?1722294893"
             alt="building" width="300"/>
            <img src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/136/202/original/rzgs2a4306011.jpg?1722295555" 
             alt="grafitti" width="300"/>
            <img src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/136/201/original/HT_abandoned_places_escher_jef_140620_3x2_1600.jpg?1722295055/>"
             alt="stair" width="300"/>
        </div>

    <hr>
     <p> Urban exploration is the exploration of manmade-- usually abandoned-- structures, ruins, or hidden hidden components of the manmadde environment.
         Photography and historical interest/documentation are heavily featured in the hobby, sometimes involving trespassing
         onto private property.</p>
    <hr>

     <a href="https://en.wikipedia.org/wiki/Urban_exploration" target="_blank">
        Learn more...
     </a>

     <button> Start Exploring </button>  

    </div>

 <footer> Coded by Klaudia Faryna</footer>

 <script>
    function changeTheme() {
        let body = document.querySelector ("body");

        if (body.classList.contains("dark")) {
            body.classList.remove("dark");
        } else {
            body.classList.add("dark");
        }
    }

    let themeButton = document.querySelector(".theme-button");
    themeButton.addEventListener("click", changeTheme);

 </script>
</body>

</html>
