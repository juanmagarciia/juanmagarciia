<h1 align="center">Hi 👋, I'm Juanma</h1>
<h3 align="center">A student backend developer from Spain</h3>

💬 Ask me about **Java, PHP, Laravel, Spring Framework, SQL, JavaFX, MVC**

📫 How to reach me **juanmangel05@gmail.com**

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://mariadb.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb" width="40" height="40"/> </a> <a href="https://spring.io/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="spring" width="40" height="40"/> </a> </p>







<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Robot Bailando</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #282c34;
            margin: 0;
            overflow: hidden;
        }.robot {
            position: relative;
            width: 150px;
            height: 200px;
        }
/* Cabeza del robot */
        .head {
            position: absolute;
            top: 0;
            left: 25px;
            width: 100px;
            height: 100px;
            background: #d4d4d4;
            border-radius: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
        }
      .eye {
            width: 20px;
            height: 20px;
            background: #000;
            border-radius: 50%;
            margin: 0 5px;
        } .eye.blink {
            animation: blink 2s infinite;
        }@keyframes blink {
            0%, 90%, 100% {
                height: 20px;
            }
            95% {
                height: 5px;
            }
        } .body {
            position: absolute;
            top: 100px;
            left: 15px;
            width: 120px;
            height: 80px;
            background: #6c6c6c;
            border-radius: 10px;
        }.arm {
            position: absolute;
            width: 20px;
            height: 60px;
            background: #6c6c6c;
            border-radius: 10px;
            top: 110px;
        }.arm.left {
            left: -25px;
            animation: swing 1s infinite alternate;
        }.arm.right {
            right: -25px;
            animation: swing 1s infinite alternate-reverse;
        }@keyframes swing {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(20deg);
            }
        } .leg {
            position: absolute;
            width: 30px;
            height: 80px;
            background: #6c6c6c;
            border-radius: 10px;
            top: 180px;
        } .leg.left {
            left: 30px;
            animation: step 0.8s infinite alternate;
        }.leg.right {
            right: 30px;
            animation: step 0.8s infinite alternate-reverse;
        } @keyframes step {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(15deg);
            }
        }
    </style>
</head>
<body>
    <div class="robot">
        <div class="head">
            <div class="eye"></div>
            <div class="eye blink"></div>
        </div>
        <div class="body"></div>
        <div class="arm left"></div>
        <div class="arm right"></div>
        <div class="leg left"></div>
        <div class="leg right"></div>
    </div>
</body>
</html>
