<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Join us to celebrate a beautiful Islamic wedding filled with love, faith, and blessings.">

    <title>Islamic Wedding Invitation - Muhsina & Abdulkudus</title>
    
    <!-- Google Fonts for Wedding Styling -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:ital,wght@0,400;0,700;1,400&family=Cormorant+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=DM+Sans:ital,opsz,wght@0,9..400,400;0,9..400,500;0,9..400,700;1,9..400,400&display=swap" rel="stylesheet">

<style>
/* =========================================
   LUXURY ISLAMIC WEDDING INVITATION
   Colour palette: Green, Wine, Gold, Ivory
========================================= */

:root {
    --green: #50C878;
    --deep-wine: #351421;
    --wine: #541b30;
    --antique-gold: #c5a45b;
    --light-gold: #ead8a6;
    --ivory: #f8f3e9;
    --white: #ffffff;
    --text-dark: #261b20;
    --muted: #766b68;
    --black: #000000;

    --heading-font: "Cormorant Garamond", Georgia, serif;
    --body-font: "DM Sans", Arial, sans-serif;
    --arabic-font: "Amiri", Georgia, serif;
}

/* =========================================
   GENERAL RESET
========================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 90px;
}

body {
    background: var(--ivory);
    color: var(--text-dark);
    font-family: var(--body-font);
    line-height: 1.7;
}

a {
    color: inherit;
    text-decoration: none;
}

button,
input,
select {
    font: inherit;
}

button,
a {
    -webkit-tap-highlight-color: transparent;
}

/* =========================================
   BACKGROUND VIDEO STYLING
========================================= */

.bg-video-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    overflow: hidden;
    z-index: -2;
}

.bg-video-container video {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.bg-video-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background: rgba(23, 17, 19, 0.85);
    z-index: -1;
    pointer-events: none;
}

/* =========================================
   NAVIGATION BAR
========================================= */

header {
    position: sticky;
    top: 0;
    z-index: 1000;
    background: rgba(23, 17, 19, 0.97);
    border-bottom: 1px solid rgba(197, 164, 91, 0.4);
    transition: all 0.3s ease-in-out;
    backdrop-filter: blur(12px);
}

nav {
    max-width: 1400px;
    margin: auto;
    padding: 20px 5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 25px;
    transition: padding 0.3s ease-in-out;
}

.logo {
    color: var(--light-gold);
    font-size: 24px;
    font-family: var(--arabic-font);
    direction: rtl;
    white-space: nowrap;
    transition: font-size 0.3s ease-in-out;
}

nav ul {
    display: flex;
    list-style: none;
    gap: 20px;
    transition: gap 0.3s ease-in-out;
}

nav ul li a {
    font-size: 13px;
    letter-spacing: 1px;
    color: var(--ivory);
    transition: font-size 0.3s ease-in-out, color 0.3s ease;
}

header.shrink {
    background: rgba(23, 17, 19, 0.98);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
}

header.shrink nav {
    padding: 10px 5%;
}

header.shrink .logo {
    font-size: 18px;
}

header.shrink nav ul {
    gap: 15px;
}

header.shrink nav ul li a {
    font-size: 11px;
}

/* =========================================
   ANIMATED BISMILLAH / NAMES MARQUEE
========================================= */

.bismillah-banner {
    overflow: hidden;
    background: var(--deep-wine);
    border-bottom: 1px solid var(--antique-gold);
    padding: 14px 0;
    white-space: nowrap;
}

.bismillah-track {
    display: flex;
    align-items: center;
    gap: 45px;
    width: max-content;
    animation: bismillahMarquee 22s linear infinite;
}

.bismillah-track span[lang="ar"] {
    color: var(--green);
    font-family: var(--arabic-font);
    font-size: 30px; /* Increased size as requested */
    line-height: 1.6;
    direction: rtl;
    animation: bismillahGlow 3s ease-in-out infinite;
}

.bismillah-divider {
    color: var(--antique-gold);
    font-size: 18px;
}

@keyframes bismillahMarquee {
    from {
        transform: translateX(0);
    }
    to {
        transform: translateX(-33.333%);
    }
}

@keyframes bismillahGlow {
    0%, 100% {
        opacity: 0.85;
        text-shadow: 0 0 6px rgba(234, 216, 166, 0.3);
    }
    50% {
        opacity: 1;
        text-shadow: 0 0 16px rgba(234, 216, 166, 0.9);
    }
}

/* =========================================
   SECTION DEFAULTS
========================================= */

section {
    padding: 100px 8%;
}

h1, h2, h3 {
    font-family: var(--heading-font);
    font-weight: 500;
    line-height: 1.15;
}

h2 {
    font-size: clamp(38px, 5vw, 60px);
    margin-bottom: 25px;
}

p {
    margin-bottom: 18px;
}

/* =========================================
   HERO / WELCOME SECTION
========================================= */

#home {
    min-height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    position: relative;
    overflow: hidden;
    color: var(--ivory);
    background: transparent;
}

#home > p:first-child {
    max-width: 650px;
    color: var(--gold);
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 3px;
    margin-bottom: 35px;
}

/* Classy updated H1 styling */
#home h1 {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 20px 0;
    color: var(--light-gold); /* Updated classy color */
    font-family: var(--heading-font);
    font-size: clamp(60px, 10vw, 120px);
    font-style: italic;
    font-weight: 700;
    line-height: 0.9;
    text-shadow: 2px 2px 8px rgba(0,0,0,0.5);
}

#home h1 span {
    color: var(--green);
    font-size: 38px;
    font-style: normal;
    font-family: var(--body-font);
    letter-spacing: 4px;
    margin: 15px 0;
    text-transform: uppercase;
}

#home p:nth-of-type(2) {
    color: #f0e6e4;
    font-size: 17px;
    line-height: 2;
    font-family: var(--heading-font);
}

#home p:nth-of-type(3) {
    color: var(--antique-gold);
    font-size: 12px;
    letter-spacing: 3px;
    margin-top: 15px;
}

#home p:nth-of-type(4) {
    color: var(--light-gold);
    font-size: 15px;
    letter-spacing: 2px;
    margin: 15px 0 30px;
}

/* =========================================
   BUTTONS
========================================= */

.button,
#home > a,
#henna-party > a,
#walima > a,
#nikkah > a,
#wedding-reception > a,
#closing > a {
    display: inline-block;
    padding: 15px 28px;
    border: 1px solid var(--antique-gold);
    background: var(--green);
    color: var(--deep-wine);
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 2px;
    text-align: center;
    transition: background 0.3s ease, color 0.3s ease, transform 0.3s ease;
}

.button:hover,
#home > a:hover,
#henna-party > a:hover,
#walima > a:hover,
#nikkah > a:hover,
#wedding-reception > a:hover,
#closing > a:hover {
    background: transparent;
    color: var(--light-gold);
    transform: translateY(-3px);
}

/* =========================================
   COUNTDOWN SECTION
========================================= */

#countdown {
    text-align: center;
    background: var(--white);
    color: var(--text-dark);
}

#countdown h2 {
    color: var(--green);
}

#countdown > p {
    color: var(--green);
}

#countdown-timer {
    max-width: 850px;
    margin: 45px auto 0;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 18px;
}

#countdown-timer > div {
    padding: 30px 15px;
    background: var(--ivory);
    border: 1px solid rgba(197, 164, 91, 0.55);
}

#countdown-timer span {
    display: block;
    color: var(--wine);
    font-family: var(--heading-font);
    font-size: 55px;
    line-height: 1.2;
}

#countdown-timer p {
    margin: 8px 0 0;
    color: var(--muted);
    font-size: 11px;
    letter-spacing: 2px;
    text-transform: uppercase;
}

/* =========================================
   EVENT SECTIONS (HENNA, WALIMA, NIKKAH, RECEPTION)
========================================= */

#henna-party, #walima, #nikkah, #wedding-reception {
    color: var(--text-dark);
    background: var(--ivory);
}

#henna-party > p:first-child,
#walima > p:first-child,
#nikkah > p:first-child,
#wedding-reception > p:first-child {
    color: var(--green);
    font-size: 12px;
    letter-spacing: 3px;
}

#henna-party h2, #walima h2, #nikkah h2, #wedding-reception h2 {
    color: var(--green);
}

/* Event Details - Black Text Fix */
.event-details {
    max-width: 700px;
    margin: 35px 0;
    border-top: 1px solid var(--antique-gold);
}

.event-details p {
    padding: 17px 0;
    margin: 0;
    border-bottom: 1px solid rgba(197, 164, 91, 0.3);
    color: var(--black) !important; /* Forces black text color */
}

.event-details strong {
    display: inline-block;
    min-width: 100px;
    color: var(--green);
}

/* =========================================
   ADDITIONAL INFORMATION
========================================= */

#details {
    text-align: center;
    background: var(--white);
}

#details h2 {
    color: var(--wine);
}

.information-card {
    max-width: 850px;
    margin: 25px auto;
    padding: 30px;
    background: var(--ivory);
    border: 1px solid rgba(197, 164, 91, 0.5);
}

.information-card h3 {
    color: var(--green);
    font-size: 32px;
    margin-bottom: 12px;
}

.information-card p {
    max-width: 650px;
    margin: auto;
    color: var(--muted);
}

#calendar-button {
    margin-top: 25px;
    padding: 15px 25px;
    border: 1px solid var(--wine);
    background: var(--green);
    color: var(--ivory);
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 2px;
    cursor: pointer;
    transition: 0.3s ease;
}

#calendar-button:hover {
    background: transparent;
    color: var(--wine);
}

/* =========================================
   RSVP SECTION
========================================= */

#rsvp {
    text-align: center;
    color: var(--text-dark);
    background: var(--ivory);
}

#rsvp h2 {
    color: var(--green);
}

#rsvp-form {
    max-width: 550px;
    margin: 35px auto 0;
    display: flex;
    flex-direction: column;
    text-align: left;
}

#rsvp-form label {
    margin: 14px 0 8px;
    color: var(--green);
    font-size: 13px;
    font-weight: 600;
}

#rsvp-form input,
#rsvp-form select {
    width: 100%;
    padding: 15px;
    border: 1px solid rgba(197, 164, 91, 0.5);
    border-radius: 0;
    background: var(--white);
    color: var(--text-dark);
    outline: none;
}

#rsvp-form input:focus,
#rsvp-form select:focus {
    border-color: var(--green);
}

#rsvp-form button {
    margin-top: 25px;
    padding: 17px;
    border: 1px solid var(--antique-gold);
    background: var(--green);
    color: var(--black);
    font-size: 12px;
    font-weight: 700;
    letter-spacing: 2px;
    cursor: pointer;
    transition: 0.3s ease;
}

#rsvp-form button:hover {
    background: var(--wine);
    color: var(--light-gold);
}

#rsvp-message {
    margin-top: 20px;
    color: var(--green);
    font-weight: 600;
}

/* =========================================
   CLOSING SECTION
========================================= */

#closing {
    text-align: center;
    color: var(--ivory);
    background: var(--deep-wine);
}

#closing > p:first-child {
    color: var(--light-gold);
    font-family: var(--arabic-font);
    font-size: 32px;
}

#closing h2 {
    color: var(--light-gold);
}

#closing h3 {
    margin-top: 45px;
    color: var(--antique-gold);
    font-size: 32px;
    line-height: 1.6;
}

/* =========================================
   FLOATING AUDIO PLAYER
========================================= */

.floating-audio-container {
    position: fixed;
    top: 20px;
    right: 20px;
    z-index: 1001;
    background: rgba(53, 20, 33, 0.95);
    border: 1px solid var(--antique-gold);
    padding: 10px 15px;
    border-radius: 30px;
    display: flex;
    align-items: center;
    gap: 10px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    backdrop-filter: blur(5px);
}

.floating-audio-container span {
    color: var(--light-gold);
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 1px;
}

.floating-audio-container audio {
    height: 32px;
    width: 200px;
}

/* =========================================
   FOOTER
========================================= */

footer {
    display: flex;
    justify-content: space-between;
    gap: 15px;
    padding: 25px 8%;
    background: #100b0e;
    color: #b6a7aa;
    font-size: 12px;
}

footer p {
    margin: 0;
}

/* =========================================
   RESPONSIVE MEDIA QUERIES
========================================= */

@media (max-width: 900px) {
    section {
        padding: 80px 6%;
    }
    nav {
        padding: 15px 4%;
    }
    #countdown-timer span {
        font-size: 45px;
    }
}

@media (max-width: 600px) {
    section {
        padding: 70px 20px;
    }
    nav {
        flex-direction: column;
        gap: 12px;
    }
    nav ul {
        justify-content: center;
        flex-wrap: wrap;
        gap: 10px 15px;
    }
    .logo {
        font-size: 20px;
    }
    #home h1 {
        font-size: clamp(45px, 14vw, 75px);
    }
    #countdown-timer {
        grid-template-columns: repeat(2, 1fr);
        gap: 12px;
    }
    #countdown-timer span {
        font-size: 38px;
    }
    .floating-audio-container {
        top: auto;
        bottom: 10px;
        right: 10px;
        left: 10px;
        justify-content: center;
        border-radius: 8px;
    }
    .floating-audio-container audio {
        width: 100%;
    }
    footer {
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
}
</style>
</head>
<body>

<!-- BACKGROUND VIDEO CONTAINER -->
<div class="bg-video-container">
    <video autoplay muted loop playsinline>
        <source src="379500_medium.mp4" type="video/mp4">
        Your browser does not support HTML5 video.
    </video>
</div>
<div class="bg-video-overlay"></div>

<!-- ANIMATED BISMILLAH BANNER -->
<div class="bismillah-banner">
    <div class="bismillah-track">
        <span lang="ar">بِسْمِ اللَّهِ الرَّحْمَٰنِ الرَّحِيمِ</span>
        <span class="bismillah-divider">✦</span>
        <span>Muhsina Musa & Abdulkudus Abdulganiyu Mayowa</span>
        <span class="bismillah-divider">✦</span>
        <span lang="ar">وَمِنْ آيَاتِهِ أَنْ خَلَقَ لَكُمْ مِنْ أَنْفُسِكُمْ أَزْوَاجًا</span>
        <span class="bismillah-divider">✦</span>
        <span>The Wedding Celebration</span>
        <span class="bismillah-divider">✦</span>
        <span lang="ar">بِسْمِ اللَّهِ الرَّحْمَٰنِ الرَّحِيمِ</span>
        <span class="bismillah-divider">✦</span>
        <span>Muhsina Musa & Abdulkudus Abdulganiyu Mayowa</span>
        <span class="bismillah-divider">✦</span>
        <span lang="ar">وَمِنْ آيَاتِهِ أَنْ خَلَقَ لَكُمْ مِنْ أَنْفُسِكُمْ أَزْوَاجًا</span>
        <span class="bismillah-divider">✦</span>
        <span>The Wedding Celebration</span>
    </div>
</div>

<!-- Add your website navigation, sections, and script tags here -->

<script>
// ========================================
// 1. STICKY HEADER SHRINK ON SCROLL
// ========================================
window.addEventListener("scroll", function () {
    const header = document.querySelector("header");
    if (window.scrollY > 50) {
        header.classList.add("shrink");
    } else {
        header.classList.remove("shrink");
    }
});

// ========================================
// 2. RSVP TO WHATSAPP
// ========================================
const rsvpForm = document.getElementById("rsvp-form");

if (rsvpForm) {
    rsvpForm.addEventListener("submit", function (event) {
        event.preventDefault();

        const name = document.getElementById("guest-name").value.trim();
        const phone = document.getElementById("guest-phone").value.trim();
        const attendance = document.getElementById("attendance").value;
        const guestCount = document.getElementById("guest-count").value;
        const messageElement = document.getElementById("rsvp-message");

        if (!name || !attendance) {
            alert("Please enter your name and select your attendance.");
            return;
        }

        const attendanceText = attendance === "attending"
            ? "Joyfully Accepts"
            : "Regretfully Declines";

        const message =
            "WEDDING RSVP 💍\n\n" +
            "Wedding of Muhsina Musa & Abdulkudus Abdulganiyu Mayowa\n" +
            "Wedding Date: Saturday, 19 December 2026\n\n" +
            "Guest Name: " + name + "\n" +
            "Guest Phone: " + (phone || "Not provided") + "\n" +
            "Attendance: " + attendanceText + "\n" +
            "Number of Guests: " + guestCount + "\n\n" +
            "Sent through the online wedding invitation.";

        const whatsappURL =
            "https://wa.me/2349033891473?text=" +
            encodeURIComponent(message);

        if (messageElement) {
            messageElement.textContent = "Opening WhatsApp to send your RSVP...";
        }

        window.location.href = whatsappURL;
    });
}
</script>

</body>
</html>
