<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Conditional Rendering Based on Dark Mode</title>
<style>
  /* CSS for hiding/showing content based on mode */
  .dark-mode-content {
    display: none;
  }
  .light-mode-content {
    display: block;
  }
</style>
</head>
<body>

<h1 align="center">Hello 👋🏼, I'm Andre Albuquerque</h1>
<h3 align="center">I study computer science at 42 Lisboa</h3>

<!-- Code to execute if it is on dark mode -->
<p align="left" class="dark-mode-content">
  <img src="https://media2.giphy.com/media/IeRw5kXQYjNYTySeq8/giphy.gif" width="205" height="150">
  <img src="https://media2.giphy.com/media/TgCoVZRnk5gZU3uqMP/giphy.gif" width="205" height="150">
  <img src="https://media4.giphy.com/media/QvpqTCiEcwtvx6wwJK/giphy.gif" width="205" height="150">
  <img src="https://media1.giphy.com/media/cOKnXRcJIznT3jT62W/giphy.gif" width="205" height="150">
</p>

<!-- Code to execute if it is on light mode -->
<p align="left" class="light-mode-content">
  <img src="https://media.giphy.com/media/R0ErGoZ2b8c7VcYr6Q/giphy.gif" width="205" height="150">
  <img src="https://media.giphy.com/media/YC7cyheiIMtZNIvsa5/giphy.gif" width="205" height="150">
  <img src="https://media.giphy.com/media/jYv31ia7eN0ZYNIwpr/giphy.gif" width="205" height="150">
  <img src="https://media.giphy.com/media/Mt1zgxr1re5M1dHopE/giphy.gif" width="205" height="150">
</p>

<!-- Other content -->
<h3>Skills 🔨</h3>
<ul>
    <li>Programming Languages: <img src="https://raw.githubusercontent.com/devicons/devicon/55609aa5bd817ff167afce0d965585c92040787a/icons/c/c-original.svg" height="40" align="center"> <img src="https://raw.githubusercontent.com/isocpp/logos/master/cpp_logo.png" height="40" align="center"> </li>
    <li>Other Skills/Tools: 
        <img src="https://cdn3.iconfinder.com/data/icons/social-media-2169/24/social_media_social_media_logo_git-256.png" height="40" align="center">
        <img src="https://user-images.githubusercontent.com/25181517/192108891-d86b6220-e232-423a-bf5f-90903e6887c3.png" height="40" align="center">
        <img src="https://user-images.githubusercontent.com/25181517/192158606-7c2ef6bd-6e04-47cf-b5bc-da2797cb5bda.png" height="40" align="center">
        <img src="https://github.com/sempostma/office365-icons/blob/master/png/1024/excel.png?raw=true" height="40" align="center">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/Notion-logo.svg/2048px-Notion-logo.svg.png" height="40" align="center">
        <img src="https://cdn-icons-png.flaticon.com/512/919/919853.png" height="40" align="center">
    </li>
</ul>

<h3 align="left">Favourite Projects 🗂️</h3>
<ul>
    <li><a href="https://github.com/AndrePortfolio/minishell">minishell</a> - Collaborated on developing a custom shell implementation in C, gaining hands-on experience in system programming and bash scripting.</li>
    <li><a href="https://github.com/AndrePortfolio/push_swap">push_swap</a> - Explored and applied various sorting algorithms, implementing them to efficiently sort stacks and enhancing my problem-solving skills.</li>
    <li><a href="https://github.com/AndrePortfolio/so_long">so_long</a> - In this project I honed my skills in graphics programming, bringing to life my first 2D mini-game inspired by the world of Pokémon.</li>
</ul>

<h3 align="left">Current Project 🔍</h3>
<p>
    <a href="https://github.com/btoksoez">cub3D</a> - Continuing to build upon the foundational skills acquired from <strong>so_long</strong>, I am now delving into the fascinating realm of raycasting techniques to simulate 3D representations. Through this project, I am not only mastering the art of applying mathematical concepts in programming but also refining my
</p>

<h3 align="left">Connect with me 🌐</h3>
<p align="left">
  <a href="mailto:fxandrealb@gmail.com" style="text-decoration: none; outline: none;">
    <img src="https://play-lh.googleusercontent.com/KSuaRLiI_FlDP8cM4MzJ23ml3og5Hxb9AapaGTMZ2GgR103mvJ3AAnoOFz1yheeQBBI=w240-h480-rw" width="40" height="40">
  </a>
  
  <a href="https://www.linkedin.com/in/andr%C3%A9-albuquerque/" target="_blank" style="text-decoration: none; outline: none;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/81/LinkedIn_icon.svg/2048px-LinkedIn_icon.svg.png" alt="LinkedIn Profile" height="40" width="40">
  </a>
</p>

<!-- Button to toggle dark mode -->
<button onclick="toggleDarkMode()">Toggle Dark Mode</button>

<script>
  // Function to toggle between light and dark mode
  function toggleDarkMode() {
    var darkModeContent = document.getElementsByClassName("dark-mode-content")[0];
    var lightModeContent = document.getElementsByClassName("light-mode-content")[0];
    
    if (darkModeContent.style.display === "none") {
      darkModeContent.style.display = "block";
      lightModeContent.style.display = "none";
      console.log("Dark mode is enabled.");
    } else {
      darkModeContent.style.display = "none";
      lightModeContent.style.display = "block";
      console.log("Light mode is enabled.");
    }

