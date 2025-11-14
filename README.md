<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Lámpara Inteligente Gamer</title>
<style>
/* RESET */
* { margin: 0; padding: 0; box-sizing: border-box; }


body {
font-family: Arial, sans-serif;
background: linear-gradient(to bottom,
#F7E7CE 0%,
#F7E7CE 45%,
#3a3a3a 45%,
#2d2d2d 55%,
#1a1a1a 65%,
#0d0d0d 75%,
#000000 85%,
#1a1a1a 100%);
color: white;
min-height: 100vh;
}


header {
background: #000000;
padding: 20px;
text-align: center;
font-size: 1.6rem;
font-weight: bold;
color: #00eaff;
position: sticky;
top: 0;
z-index: 10;
transition: background 0.3s ease;
}


header.scrolled {
background: rgba(0, 0, 0, 0.85);
backdrop-filter: blur(4px);
}


.container {
padding: 20px;
display: flex;
flex-wrap: wrap;
justify-content: center;
gap: 20px;
}


.product {
background: #1a1a1a;
padding: 15px;
border-radius: 10px;
width: 100%;
max-width: 350px;
}


.product img {
width: 100%;
height: auto;
border-radius: 8px;
}


button {
width: 100%;
padding: 12px;
background: #00eaff;
border: none;
color: black;
font-weight: bold;
border-radius: 5px;
cursor: pointer;
margin-top: 10px;
