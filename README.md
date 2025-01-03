<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your GitHub Profile</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Animated Header with Profile and Wallpaper -->
    <header>
        <div class="background"></div>
        <div class="content">
            <h1>Welcome to My GitHub!</h1>
            <div class="profile">
                <img src="your-profile-image.jpg" alt="Your Profile Picture" class="profile-img">
                <p class="name">Your Name</p>
                <p class="bio">A passionate developer, creating cool projects with a cyberpunk vibe!</p>
            </div>
        </div>
    </header>

    <!-- Animated Wall of Projects/Posts Section -->
    <section class="projects">
        <h2>Latest Projects</h2>
        <div class="project-card">
            <h3>Project 1</h3>
            <p>A short description of Project 1.</p>
        </div>
        <div class="project-card">
            <h3>Project 2</h3>
            <p>A short description of Project 2.</p>
        </div>
        <!-- Add more project cards here -->
    </section>

    <footer>
        <p>Thank you for visiting my profile!</p>
    </footer>
</body>
</html>
/* Basic styles for the page */
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    color: white;
    background-color: black;
    overflow: hidden;
}

/* Animation for background */
@keyframes backgroundEffect {
    0% {
        transform: scale(1.1);
    }
    50% {
        transform: scale(1.05);
    }
    100% {
        transform: scale(1.1);
    }
}

/* Background animation */
.background {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: url('your-live-wallpaper-url.gif');
    background-size: cover;
    animation: backgroundEffect 15s infinite;
    z-index: -1;
}

/* Content styling */
header {
    text-align: center;
    padding-top: 100px;
}

h1 {
    font-size: 3em;
    text-shadow: 0px 0px 10px rgba(255, 0, 255, 0.8);
    animation: fadeIn 3s ease-in-out;
}

.profile {
    display: inline-block;
    text-align: center;
    margin-top: 20px;
}

.profile-img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    border: 5px solid rgba(255, 0, 255, 0.5);
    box-shadow: 0 0 15px rgba(255, 0, 255, 0.8);
    animation: bounce 1.5s infinite;
}

.name {
    font-size: 1.5em;
    margin-top: 15px;
}

.bio {
    font-size: 1.2em;
    color: #ff66ff;
    margin-top: 10px;
}

/* Fade-in animation */
@keyframes fadeIn {
    0% {
        opacity: 0;
    }
    100% {
        opacity: 1;
    }
}

/* Bounce effect for profile image */
@keyframes bounce {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-10px);
    }
}

/* Section styling */
.projects {
    margin: 50px;
    text-align: center;
}

.project-card {
    background: rgba(255, 0, 255, 0.2);
    padding: 20px;
    margin: 20px;
    border-radius: 10px;
    box-shadow: 0px 0px 10px rgba(255, 0, 255, 0.8);
    animation: fadeIn 3s ease-in-out;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: rgba(0, 0, 0, 0.8);
    color: white;
}

