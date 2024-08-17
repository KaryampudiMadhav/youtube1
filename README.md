# youtube1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Youtube</title>
    <style>
        .content{
            display: inline-block;
            width: 100%;
        }
        body{
            margin: 0px;
            padding-top:60px; 
            padding-left: 70px;
            background-color: white;
        }
        .container{
            width: 350px;
            display: inline-block;
        }
        .img1{
            margin-top: 3px;
            width: 350px;
            height: 200px;
            display: inline-block;
            position: relative;
            z-index: 0;
        } 
 
        .profile{
            width: 40px;
            border-radius: 50px;
        }
        .first-para{
            margin-top: 3px;
            font-weight: bold;
        }
        .css-grid{
            display:grid;
            grid-template-columns: 50px 1fr;
        }
        .content p{
            margin: 2px 0;
        }
        .total-grid{
            display: grid;
            grid-template-columns: 1fr 1fr  1fr 1fr;
        }
        @media (max-width: 750px){
            .total-grid{
                grid-template-columns: 1fr 1fr;
            }
        }
        @media (min-width: 751px) and (max-width: 999px){
            .total-grid{
                grid-template-columns: 1fr 1fr 1fr;
            }
        }
        .header{
            background-color: white;
            top: 0;
            right: 0;
            left: 0;
            position: fixed;
            padding-top: 10px;
            height: 30px;
            display: flex;
            justify-content: space-between;
            padding-bottom: 10px;
            border-bottom-style: solid;
            border-bottom-width: 1px;
            border-bottom-color: rgb(204, 201, 201);
            z-index: 100;
        }
        .hanger{
            margin-left: 10px;
            width: 25px;
        }
        .start{
            width: 300px;
            display: flex;
            align-items: center;
        }
        .logo{
            margin-left: 15px;
            margin-right: 50px;
            height: 30px;
            width: 100px;
        }
        .search-img{
            margin-left: 2px;
            height: 30px;
            width: 20px;
        }
        .search-button{
            margin-left: -1px;
            flex: 1;
            height: 41px;
            width: 50px;
            border-width: 1px;
            border-style: solid;
            border-color: rgb(184, 181, 181);
            border-radius: 2px;
        }
        .middle{
            display: flex;
            align-items: center;
            width: 500px;
        }
        .text::placeholder{
            font-weight: bold;
            font-family: Arial, Helvetica, sans-serif;
            font-size: 18px;
        }
        .time{
            position: absolute;
            bottom: 10px;
            right: 10px;
            background-color: black;
            color: white;
            border-radius: 2px;
            padding-left: 3px;
            padding-right: 3px;
            font-weight: bold;
            font-size: 15px;
            font-family: Arial, Helvetica, sans-serif;
        }    
        .text{
            flex: 1;
            width: 300px;
            padding-top: 2px;
            border-width: 1px;
            border-style: solid;
            border-color: rgb(204, 201, 201);
            border-radius: 2px;
            font-size: 15px;
            height: 36px;
            padding-left: 10px;
        }
       .last{
        flex-shrink: 0;
        width: 200px;
        display: flex;
        justify-content: space-between;
        align-items: center;
       }
       .left-item1,.left-item2,.left-item3{
        width: 30px;
        margin-right: 10px;
       }
       .voice{
        margin-left: 10px;
        width: 30px;
       }
       .voice-button{
        background-color: white;
        border: none;
        border-radius: 50px;
       }
       .video-button,.icon-button,.profile-button{
        border: none;
        background-color: white;
       }
       .profile-button{
        border-radius: 50px;
       }
       .notification-button{
        width: 25px;
        border: none;
        background-color: white;
       }
       .number{
           position: absolute;
           top: 0px;
           left: 12px;
           background-color: rgb(100, 4, 4);
           border-radius: 50px;
           color: white;
           font-weight: bold;
           width: 10px;
           padding-left: 6px;
           padding-right: 3px;
       }
       .sub{
        position: relative;
       }
       .notification{
        width: 30px;
       }
     .side-contain{
        width: 67px;
        position: fixed;
        top: 50px;
        left: 0px;
        height: 500px;
        background-color: white;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        text-align: center;
     }
     .home-icon{
        margin-top: 10px;
        width: 30px;
     }
    .side-contain div{
        font-size: 10px;
        font-family: Arial, Helvetica, sans-serif;
        font-weight: 500px;
     }
    </style>
</head>
<body>
    <div class="header">
       <div class="start">
        <div><img  src="hamburger-menu.svg" class="hanger"></div>
        <div><img src="youtube-logo.svg" class="logo"></div>
       </div>
        <div class="middle">
            <div><input class="text" type="text" placeholder="Search"></div>
            <div><button class="search-button"><img src="search.svg" class="search-img" ></button></div>
            <div><button class="voice-button"><img src="voice-search-icon.svg"  class="voice"></button></div>
        </div>
        <div class="last">
            <div><button class="video-button"><img src="upload.svg" class="left-item1"></button></div>
            <div class="sub">
            <img src="notifications.svg" class="notification-button">
            <div class="number">3</div>
            </div>
            <div><button class="icon-button"><img src="youtube-apps.svg" class="left-item2" ></button></div>
            <div><button class="profile-button"><img src="my-channel.jpeg" class="left-item3" ></button></div>
        </div>
    </div>
    <div class="side-contain">
   <div class="left-side">
    <img src="home.svg" class="home-icon">
    <div class="writing">Home</div>
   </div>
   <div class="left-side"><img src="explore.svg" class="home-icon">
    <div class="writing">Explore</div>
    </div>
   <div class="left-side"><img src="originals.svg" class="home-icon">
    <div class="writing">Originals</div>
   </div>
   <div class="left-side"><img src="subscriptions.svg" class="home-icon">
    <div class="writing">Youtube Music</div>
   </div>
   <div class="left-side"><img src="youtube-music.svg" class="home-icon">
    <div class="writing">Subcriptions</div>
    </div>
   <div class="left-side"><img src="library.svg" class="home-icon">
    <div class="writing">Library</div>
   </div>
    </div>
    <div class="total-grid">
        <div class="container">
            <div class="img1">
                    <img src="thumbnail-1.webp" class="img1">
                    <div class="time">4:00</div>
            </div>
            <div class="css-grid">       
              <div class="profile-div">
                <img src="channel-1.jpeg" class="profile">
            </div>
           <div class="content">
            <div class="row1"><p class="first-para">Talking Tech and AI with Google CEO Sundar Pichai!</p>
            </div>
            <div ><p>Marques Brownlee &#10004</p></div>
            <div><p>3.4M views · 6 months ago</p></div>
            </div>
        </div>
       </div>
        <div class="container">
        <div class="img1">
             <img src="thumbnail-2.webp" class="img1">
             <div class="time">5:30</div>
        </div>
        <div class="css-grid">  
                <div class="profile-div">
                <img src="channel-2.jpeg" class="profile">
                 </div>
                <div class="content">
                <div><p class="first-para">Try Not To Laugh Challenge #9p></div>
                <div> <p>Markiplier &#10004</p></div>
                <div> <p>19M views · 4 years ago</p></div>  
        </div>
        </div>
        </div>
        <div class="container">
            <div class="img1">
                    <img src="thumbnail-3.webp" class="img1">
                    <div class="time">7:90</div>
            </div>
            <div class="css-grid">       
              <div class="profile-div">
                <img src="channel-3.jpeg" class="profile">
            </div>
           <div class="content">
            <div class="row1"><p class="first-para">
                Crazy Tik Toks Taken Moments Before DISASTER</p>
            </div>
            <div ><p>SSSniperWolf</p></div>
            <div><p>12M views · 1 year ago</p></div>
            </div>
        </div>
       </div>
        <div class="container">
        <div class="img1">
             <img src="thumbnail-4.webp" class="img1">
             <div class="time">2:60</div>
        </div>
        <div class="css-grid">  
                <div class="profile-div">
                <img src="channel-4.jpeg" class="profile">
                 </div>
                <div class="content">
                <div><p class="first-para">The Simplest Math Problem No One Can Solve - Collatz Conjecture</p></div>
                <div> <p>Veritasium</p></div>
                <div> <p>18M views · 4 months ago</p></div>  
        </div>
        </div>
        </div>
        <div class="container">
            <div class="img1">
                    <img src="thumbnail-5.webp" class="img1">
                    <div class="time">8:90</div>
            </div>
            <div class="css-grid">       
              <div class="profile-div">
                <img src="channel-5.jpeg" class="profile">
            </div>
           <div class="content">
            <div class="row1"><p class="first-para">Kadane's Algorithm to Maximum Sum Subarray Problem</p>
            </div>
            <div ><p>CS Dojo</p></div>
            <div><p>519K views · 5 years ago</p></div>
            </div>
        </div>
       </div>
        <div class="container">
        <div class="img1">
             <img src="thumbnail-6.webp" class="img1">
             <div class="time">3:00</div>
        </div>
        <div class="css-grid">  
                <div class="profile-div">
                <img src="channel-6.jpeg" class="profile">
                 </div>
                <div class="content">
                <div><p class="first-para">
                    Anything You Can Fit In The Circle I’ll Pay For</p></div>
                <div> <p>MrBeast</p></div>
                <div> <p>141M views · 1 year ago</p></div>  
        </div>
        </div>
        </div>
        <div class="container">
            <div class="img1">
                    <img src="thumbnail-7.webp" class="img1">
                    <div class="time">9:00</div>
            </div>
            <div class="css-grid">       
              <div class="profile-div">
                <img src="channel-7.jpeg" class="profile">
            </div>
           <div class="content">
            <div class="row1"><p class="first-para">Why Planes Don't Fly Over Tibet</p>
            </div>
            <div ><p>RealLifeLore</p></div>
            <div><p>6.6M views · 1 year ago</p></div>
            </div>
        </div>
       </div>
       <div class="container">
        <div class="img1">
                <img src="thumbnail-8.webp" class="img1">
                <div class="time">4:00</div>
        </div>
        <div class="css-grid">       
          <div class="profile-div">
            <img src="channel-8.jpeg" class="profile">
        </div>
       <div class="content">
        <div class="row1"><p class="first-para">Inside The World's Biggest Passenger Plane</p>
        </div>
        <div ><p>Tech Vision</p></div>
        <div><p>3.7M views · 10 months ago</p></div>
        </div>
    </div>
    </div>
    <div class="container">
        <div class="img1">
                <img src="thumbnail-9.webp" class="img1">
                <div class="time">4:00</div>
        </div>
        <div class="css-grid">      
          <div class="profile-div">
            <img src="channel-9.jpeg" class="profile">
        </div>
       <div class="content">
        <div class="row1"><p class="first-para">The SECRET to Super Human STRENGTH</p>
        </div>
        <div ><p>ThenX</p></div>
        <div><p>20M views · 3 year ago</p></div>
        </div>
    </div>
   </div>
    <div class="container">
    <div class="img1">
         <img src="thumbnail-10.webp" class="img1">
         <div class="time">4:00</div>
    </div>
    <div class="css-grid">  
            <div class="profile-div">
            <img src="channel-10.jpeg" class="profile">
             </div>
            <div class="content">
            <div><p class="first-para">
                How The World's Largest Cruise Ship Makes 30,000 Meals Every Day</p></div>
            <div> <p>Business Insider</p></div>
            <div> <p>14M views · 1 year ago</p></div>  
    </div>
    </div>
    </div>
    <div class="container">
        <div class="img1">
                <img src="thumbnail-11.webp" class="img1">
                <div class="time">4:00</div>
        </div>
        <div class="css-grid">       
          <div class="profile-div">
            <img src="channel-11.jpeg" class="profile">
        </div>
       <div class="content">
        <div class="row1"><p class="first-para">
            Dubai's Crazy Underwater Train and Other Things #Only in Dubai</p>
        </div>
        <div ><p>Destination Tips</p></div>
        <div><p>3M views · 1 year ago</p></div>
        </div>
    </div>
   </div>
    <div class="container">
    <div class="img1">
         <img src="thumbnail-12.webp" class="img1">
         <div class="time">4:00</div>
    </div>
    <div class="css-grid">  
            <div class="profile-div">
            <img src="channel-12.jpeg" class="profile">
             </div>
            <div class="content">
            <div><p class="first-para">What would happen if you didn’t drink water? - Mia Nacamulli</p></div>
            <div> <p>TED-Ed</p></div>
            <div> <p>12M views · 5 years ago</p></div>  
    </div>
    </div>
    </div>
    </div> 
</body>
</html>
