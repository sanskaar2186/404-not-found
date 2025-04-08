<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Alpine - Mountain Climbing Trips</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400;700;900&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body, html {
      font-family: 'Raleway', sans-serif;
      color: rgb(224, 237, 223);
      height: 100%;
    }

    body {
      background: url('C:\Users\ayman\OneDrive\Pictures\Screenshots\Screenshot 2025-04-08 194827.png') no-repeat center center/cover;
      height: 100vh;

      position: relative;
    }

    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background-color: rgba(114, 30, 30, 0.4);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      z-index: 10;
    }

    .logo {
      font-size: 24px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo::before {
      content: '🌲';
      font-size: 24px;
    }

    .nav-items select {
      background: transparent;
      border: none;
      color: white;
      font-size: 16px;
      margin: 0 10px;
      cursor: pointer;
    }

    .nav-items select:focus {
      outline: none;
    }

    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 100px 60px;
      background: rgba(0, 0, 0, 0.3);
    }

    .search-bar {
      margin-bottom: 30px;
      display: flex;
      align-items: center;
    }

    .search-bar input {
      padding: 10px 20px;
      border-radius: 30px;
      border: none;
      width: 300px;
      font-size: 16px;
      outline: none;
    }

    h1 {
      font-size: 48px;
      font-weight: 900;
    }

    h2 {
      font-size: 32px;
      font-weight: 700;
      margin-bottom: 20px;
    }

    .view-program {
      margin-top: 20px;
      padding: 10px 30px;
      font-size: 16px;
      border: 2px solid white;
      border-radius: 30px;
      background-color: transparent;
      color: white;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .view-program:hover {
      background-color: white;
      color: black;
    }

    .video-section {
      position: absolute;
      top: 50%;
      right: 100px;
      transform: translateY(-50%);
      display: flex;
      align-items: center;
      gap: 20px;
    }

    .video-section .play-btn {
      width: 60px;
      height: 60px;
      border: 2px solid white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
    }

    .video-section .play-btn::before {
      content: '▶';
      font-size: 20px;
    }

    .video-section .text {
      max-width: 250px;
    }

    .video-section .text h3 {
      margin-bottom: 8px;
    }

    .about {
      position: absolute;
      bottom: 40px;
      left: 60px;
      max-width: 400px;
    }

    .about p {
      font-size: 14px;
      margin-bottom: 10px;
    }

    .about a {
      color: white;
      font-size: 14px;
      text-decoration: underline;
    }

    .socials {
      position: absolute;
      bottom: 40px;
      left: 20px;
      display: flex;
      flex-direction: column;
      gap: 15px;
      font-size: 18px;
    }

    .socials a {
      color: rgb(255, 255, 255);
      text-decoration: none;
    }

    @media (max-width: 768px) {
      .hero {
        padding: 100px 20px;
      }

      .video-section {
        position: static;
        transform: none;
        margin-top: 30px;
        flex-direction: column;
        align-items: flex-start;
      }

      .video-section .text {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>

  <nav>
    <div class="logo">no planes,just planes</div>
    <div class="nav-items">
      <select>
        <option>TRAVELLER TYPE</option>
        <option>Solo</option>
        <option>Family</option>
      </select>
      <select>
        <option>COUPLE</option>
        <option>Yes</option>
        <option>No</option>
      </select>
      <select>
        <option>PROGRAM</option>
        <option>Hiking</option>
        <option>Climbing</option>
      </select>
      <select>
        <option>MOUNTAINING</option>
        <option>Beginner</option>
        <option>Pro</option>
      </select>
      <select>
        <option>SET LOCATION</option>
        <option>Himalayas</option>
        <option>Alps</option>
      </select>
    </div>
  </nav>

  <div class="hero">
    <div class="search-bar">
      <input type="text" placeholder="Search...">
    </div>
    <h1>Mountain</h1>
    <h2>Climbing Trips & Tours</h2>
    <button class="view-program">VIEW PROGRAM</button>
  </div>

  <div class="video-section">
    <div class="play-btn" onclick="playVideo()"></div>
    <div class="text">
      <h3>Watch Videos</h3>
      <p>Lorem Ipsum Dolor Sit Amet, Consectetur Adipisicing Elit, Sed Do Eiusmod Tempor Incididunt Ut Labore Et Dolore Magna Aliqua.</p>
    </div>
  </div>

  <div class="about">
    <p>Lorem Ipsum Dolor Sit Amet, Consectetur Adipisicing Elit, Sed Do Eiusmod Tempor Incididunt Ut Labore Et Dolore Magna Aliqua.</p>
    <a href="#">READ MORE...</a>
  </div>

  <div class="socials">
    <a href="#">📘</a>
    <a href="#">📸</a>
    <a href="#">🐦</a>
    <a href="#">▶️</a>
  </div>

  <script>
    function playVideo() {
      alert('Video player will open here.');
    }
  </script>

</body>
</html>
