<! --html codes of accordions-->
<html>
    <head>
        <link rel="stylesheet" href="index.css">
    </head>
    <body>
        <h1>Tech Staff</h1>
    <ul class="accordion">
    <li>
    <img src="larson.jpg" /> 
    <div class="content">
    <span>
    <h2>Brie Larson</h2> 
    <p>Frontend</p>
    </span>
    </div>
    </li>
    <li>
    <img src="olsen.webp" /> 
    <div class="content">
    <span>
    <h2>Elizabeth Olsen</h2>
    <p>Blockchain Engineer</p>
    </span>
    </div>
    </li>
    <li>
        <img src="scarlett.jpg" /> 
        <div class="content">
        <span>
        <h2>Scarlett Johansson</h2>
        <p>AI Engineer</p>
        </span>
        </div>
        </li>
        <li>
            <img src="lana.jpg" /> 
            <div class="content">
            <span>
            <h2>Lana Del Rey</h2>
            <p>Test Engineer</p>
            </span>
            </div>
            </li>
            <li>
                <img src="monica.webp" /> 
                <div class="content">
                <span>
                <h2>Monica Belluci</h2>
                <p>Backend</p>
                </span>
                </div>
                </li>
    </ul>
    </body>
    </html>



 CSS part;
 h1{
    margin-bottom: 20;
}
.accordion:hover { gap: 25;
}
* {
margin: 0;
padding: 0;
box-sizing: border-box;
}
body {
min-height: 100vh;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center; background: #3a3544;
text-align: center;
font-family: "Poppins";
}
.accordion {
width: 100%;
display: flex;
justify-content: center;
height: 400px;
gap:16px;
transition: 0.3s;


}



.accordion h2 { font-weight: 400; 
    font-size: 24px; 
    line-height: 45px;
    border-bottom: 2px solid #fff; 
    white-space: nowrap;
}


.accordion li {

position: relative; 
overflow: hidden; 
flex: 0 0 80px;
border-radius: 50px; 
opacity: 0.75; 
cursor: pointer;
}

.accordion li img {
position: absolute; 
top: 50%;
left: 50%;
translate: -50% -50%;
width: 100%;
height: 100%;
object-fit: cover;
}


.accordion li,
.accordion li img,
.accordion li .content,
.accordion li .content span { transition: 0.3s;
}
.accordion li .content {
position: absolute;
top: 0;
left: 0;
right: 0;
bottom: 0;
z-index: 1;
color: #fff;
padding: 15px;
background: #02022e;
background:
linear-gradient(
0deg,
rgb(
0 0 0 /70%
) 10%,
rgb(
255 255 255 / 0%
) 100%
);
opacity: 0;
visibility:hidden;
}

.accordion li 
.content span { 
    position: absolute; 
    z-index: 3; 
    left: 50%; 
    bottom: 50px;
translate: -300px 0;
 visibility: hidden; 
 opacity: 0;
}
.accordion li:hover {
flex: 0 1 260px;
scale: 1.1;
z-index: 10;
opacity: 1;
}
.accordion li:hover
.content {
    opacity: 1;
    visibility: visible;
}


.accordion li:hover span {
    translate: -50% 0;
    opacity: 1;
    visibility: visible;
}
