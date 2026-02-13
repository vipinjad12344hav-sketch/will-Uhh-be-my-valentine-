# will-Uhh-be-my-valentine-?!!❤
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Valentine Saee 💖</title>

<style>
body {
    margin: 0;
    padding: 0;
    background: linear-gradient(135deg, #ff4e8a, #ff99cc);
    font-family: 'Segoe UI', sans-serif;
    text-align: center;
    overflow-x: hidden;
    color: white;
}

/* Title */
h1 {
    margin-top: 50px;
    font-size: 38px;
    animation: glow 2s infinite alternate;
}

@keyframes glow {
    from { text-shadow: 0 0 10px white; }
    to { text-shadow: 0 0 25px #fff, 0 0 40px pink; }
}

/* Image Styling */
.photo-container {
    margin-top: 30px;
}

.photo-container img {
    width: 220px;
    height: 220px;
    object-fit: cover;
    border-radius: 50%;
    border: 5px solid white;
    box-shadow: 0 0 30px white;
    animation: pulse 2s infinite;
}

@keyframes pulse {
    0% { box-shadow: 0 0 20px white; }
    50% { box-shadow: 0 0 40px pink; }
    100% { box-shadow: 0 0 20px white; }
}

p {
    font-size: 20px;
    margin-top: 20px;
}

/* Button */
button {
    padding: 12px 25px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    background: white;
    color: #ff4e8a;
    cursor: pointer;
    margin-top: 25px;
    transition: 0.3s;
}

button:hover {
    background: #ff4e8a;
    color: white;
    transform: scale(1.1);
}

/* Surprise */
#surprise {
    display: none;
    margin-top: 20px;
    font-size: 22px;
    animation: pop 1s ease forwards;
}

@keyframes pop {
    from { transform: scale(0); opacity: 0; }
    to { transform: scale(1); opacity: 1; }
}

/* Floating Hearts */
.heart {
    position: fixed;
    bottom: -20px;
    font-size: 20px;
    animation: float 6s linear infinite;
}

@keyframes float {
    0% { transform: translateY(0) rotate(0deg); opacity: 1; }
    100% { transform: translateY(-100vh) rotate(360deg); opacity: 0; }
}
</style>
</head>

<body>

<h1>Happy Valentine’s Day Saee 💖</h1>

<div class="photo-container">
    <!-- Replace photo.jpg with your image file name -->
    <img src="photo.jpg" alt="Saee ❤️">
</div>

<p>My Sweet Cupcake 🧁<br>
You are my happiness, my forever, my everything 💞</p>

<button onclick="showSurprise()">Click for Surprise 🎁</button>

<div id="surprise">
    🌹 Saee, will you be my forever Valentine? 💍❤️  
</div>

<script>
function showSurprise() {
    document.getElementById("surprise").style.display = "block";
}

function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "💖";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 15 + "px";
    heart.style.animationDuration = Math.random() * 3 + 3 + "s";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 6000);
}

setInterval(createHeart, 300);
</script>

</body>
</html>
