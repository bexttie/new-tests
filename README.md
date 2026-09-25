
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>rebeca | profile</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,500;1,400&display=swap" rel="stylesheet">

    <style>
        /* =========================================
           RESET
        ======================================== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        html {
            scroll-behavior: smooth;
        }
        body {
            background: #ffdfdf;
            color: #a04731;
            font-family: Arial, Helvetica, sans-serif;
            font-size: 12px;
            line-height: 1.3;
            padding: 24px 12px 40px;
        }
        a {
            color: inherit;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }

        img {
            display: block;
            max-width: 100%;
        }

        button {
            font-family: inherit;
            cursor: pointer;
        }
        /* =========================================
           MAIN PAGE
        ========================================= */
        .page {
            width: 100%;
            max-width: 420px;
            margin: 0 auto;
        }
        /* =========================================
           PROFILE HEADER
        ========================================= */
        .profile {
            display: flex;
            align-items: center;
            gap: 18px;
            margin-bottom: 7px;
        }
        .profile-avatar {
            width: 70px;
            height: 90px;
            flex-shrink: 0;
            border-radius: 10%;
            overflow: hidden;
            background: #1a1818;
        }

        .profile-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .profile-info {
            min-width: 0;
        }
        .profile-name {
            font-family: Inter, 'inter', serif;
            font-size: 21px;
            font-weight: bold;
            color: #f00070;
            line-height: 1.3;
        }
        .profile-name .dot {
            color: #be0461;
        }
        .profile-handle {
            font-family: Inter, 'inter', serif;
            font-size: 18px;
            font-weight: normal;
            color: #69b6ff; rgb(255, 42, 0)rgb(158, 26, 0)rgb(158, 0, 87)
        }
        .profile-description {
            margin-top: 10px;
            font-family: Inter, 'inter', serif;
            font-size: 13px;
            line-height: 1.45;
            color: #009af3;
        }
        .profile-description a {
            text-decoration: underline;
            text-underline-offset: 2px;
        }

        .profile-note {

            color: #00e40bfb;
            font-size: 11.5px;
            margin-top: 2px;
        }
        .profile-actions {
            display: flex;
            gap: 10px;
            margin-bottom: 16px;
        }
        .action-button {
            width: 130px;
            height: 37px;
            border: none;
            border-radius: 3px;
            background: #030303;
            color: #ffacac;
            font-size: 14px;
            font-weight: bold;
            text-align: center;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .action-button:hover {
            background: #928885;
            text-decoration: none;
        }
        .content-grid {
            display: grid;
            grid-template-columns: minmax(0, 1fr) minmax(0, 0.7fr);
            gap: 20px;
            align-items: start;
        }
        .left-column,
        .right-column {
            min-width: 0;
        }
        .text-box {
            border: 1px solid #007aec;
            padding: 7px 8px;
            margin-bottom: 10px;
            color: #5d00d6;
            font-family: inter bold;
            font-size: 11px;
            line-height: 1.18;
            min-height: 80px;
        }
        .text-box p {
            margin-bottom: 5px;
        }
        .text-box p:last-child {
            margin-bottom: 0;
        }
        .text-box a {
            text-decoration: underline;
        }
 
        .section-title {
            font-family: Inter, 'Inter', serif;
            font-size: 19px;
            font-weight: normal;
            line-height: 1.2;
            color: #ff009d;
            margin-bottom: 10px;
        }
        .section-line {
            width: 100%;
            height: 2px;
            background: #f300a2 50%;
            margin-bottom: 14px;
        }
        .friend-list {
            display: flex;
            flex-direction: column;
            gap: 13px;
        }
        .friend {
            display: flex;
            align-items: flex-start;
            gap: 10px;
            min-width: 0;
        }
        .friend-avatar {
            width: 58px;
            height: 58px;
            flex-shrink: 0;
            border-radius: 80%;
            overflow: hidden;
            background: #1c1a1a;
        }
        .friend-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .friend-info {
            min-width: 0;
            padding-top: 2px;
        }
        .friend-name {
            font-size: 12px;
            font-weight: bold;
            color: #f30096;
            margin-bottom: 2px;
        }
        .friend-details {
            font-size: 11px;
            line-height: 1.3;
            color: #13e400e5;
            overflow-wrap: anywhere;
        }
        .friend-details .muted {
            color: #9191db;
        }
        .playlists {
            margin-top: 12px;
        }
        .playlist-header {
            font-family: Inter bold, 'Inter bold', serif;
            font-size: 19px;
            font-weight: normal;
            color: #e6006b;
            margin-bottom: 8px;
        }
        .playlist-line {
            width: 100%;
            height: 3px;
            background: #ff05ac4b;
            margin-bottom: 10px;
        }
        .playlist-grid {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 5px;
        }
        .playlist-card {
            min-width: 0;
        }
        .playlist-image {
            width: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            background: #1b1919;
        }
        .playlist-title {
            margin-top: 8px;
            font-size: 12px;
            font-weight: bold;
            line-height: 1.2;
            color: #550043;
        }
        .playlist-description {
            margin-top: 7px;
            font-size: 11px;
            line-height: 1.4;
            color: #6d002d;
        }
        @media (max-width: 360px) {
            body {
                padding: 18px 10px 30px;
            }
            .profile {
                gap: 12px;
            }
            .profile-avatar {
                width: 78px;
                height: 78px;
            }
            .profile-name {
                font-size: 18px;
            }
            .profile-handle {
                font-size: 15px;
            }
            .profile-description {
                font-size: 12px;
            }
            .content-grid {
                gap: 10px;
            }
            .friend {
                gap: 7px;
            }
            .friend-avatar {
                width: 48px;
                height: 48px;
            }
            .section-title,
            .playlist-header {
                font-size: 17px;
            }
            .playlist-grid {
                gap: 6px;
            }
        }
    </style>
</head>
<body>
    <main class="page">
        <header class="profile">
            <div class="profile-avatar">
                <img src="https://i.pinimg.com/736x/88/ec/7a/88ec7a0d3c35fcac13e39b77f67c0be6.jpg" alt="Profile picture">
            </div>
            <div class="profile-info">
                <h1 class="profile-name">
                    rebeca zhu <span class="dot">·</span> 
                    <span class="profile-handle">@bexttie</span>
                </h1>
                <div class="profile-description">
                    23 -- >u- <br> i speak eng, ptbr, cn, es, fr and it 
                    <br>
                    <a href="#">main</a>
                    <a href="#">private</a>
                    <a href="#">spotify</a>
                    <a href="#">art site</a>
                </div>
                <p class="profile-note">
                    she/her 
                </p>
            </div>
        </header>
        <div class="profile-actions">
            <a href="#" class="action-button">
                Love
            </a>
            <a href="#" class="action-button">
                Me
            </a>
        </div>
        <div class="content-grid">
            <section class="left-column">
                <div class="text-box">
                    <p>
                        hello there, just so you know, i am mad and i do day dream a lot
                    </p>
                </div>
                <div class="text-box">
                    <p>
                        i wont follow if ur a weirdo
                        heavy/no interaction, 
                        (im selective)
                    </p>
                </div>
            </section>
            <section class="right-column">
                <h2 class="section-title">
                    Friend Activity
                </h2>
                <div class="section-line"></div>
                <div class="friend-list">
                    <article class="friend">
                        <div class="friend-avatar">
                            <img src="https://i.pinimg.com/736x/c2/24/71/c22471ea3827c5535386bb6e839218ee.jpg" alt="Friend avatar1">
                        </div>
                        <div class="friend-info">
                            <p class="friend-name">
                                honorato
                            </p>
                            <p class="friend-details">
                                awu
                                <br>
                               LiSa
                                <br>
                                <span class="muted">
                                    ♫ gurenge...
                                </span>
                            </p>
                </div>
                    </article>
                    <!-- FRIEND 2 -->
                    <article class="friend">
                        <div class="friend-avatar">
                            <img src="https://i.pinimg.com/736x/7a/62/bd/7a62bd7d67b71e69dca644fc5ec51e1b.jpg" alt="Friend avatar">
                </div>
                        <div class="friend-info">
                            <p class="friend-name">
                                hollow
                            </p>
                            <p class="friend-details">
                                boludo
                                <br>
                                Linkin Park
                                <br>
                                <span class="muted">
                                    ♫ castle of glass...
                                </span>
                            </p>
                        </div>
                    </article>
                    <article class="friend">
                        <div class="friend-avatar">
                            <img src="https://i.pinimg.com/736x/6e/b7/85/6eb7857c523d1609fd7b730d1a65528c.jpg" alt="Friend avatar">
                        </div>
                        <div class="friend-info">
                            <p class="friend-name">
                                bararaq
                            </p>
                            <p class="friend-details">
                                mono pantheon
                                <br>
                                Ado
                                <br>
                                <span class="muted">
                                    ♫ Flower...
                                </span>
                            </p>
                        </div>
                    </article>
                </div>
            </section>
        </div>
        <section class="playlists">
            <h2 class="playlist-header">
                about me
            </h2>
            <div class="playlist-line"></div>
            <div class="playlist-grid">
                <!-- PLAYLIST 1 -->
                <article class="playlist-card">
                    <img
                        class="playlist-image"
                        src="https://i.pinimg.com/1200x/55/b6/29/55b6296cd671aaba46c48e2e25933189.jpg"
                        alt="Love zone playlist"
                    >
                    <h3 class="playlist-title">
                        songs
                    </h3>
                    <p class="playlist-description">
                    Aclame ao Senhor - Felipe Rodrigues<br>
                    Back to me - The Rose<br>You'll be in my heart - Tarzan
                        <br>
                    one of my favourite songs
                    </p>
                </article>
                <article class="playlist-card">
                    <img
                        class="playlist-image"
                        src="https://i.pinimg.com/736x/25/3e/e9/253ee983d2ebc414f8f70d253f2ce5e0.jpg"
                        alt="Mmmmmhm playlist"
                    >
                    <class="playlist-title">
                        <h3>programms I use</h3>
                    class="playlist-description"
                        <p>VScode, C#, Unreal Engine, CSP, IbisPaint</p>
                        <b>
                </article>
                <article class="playlist-card">
                    <img
                        class="playlist-image"
                        src="https://i.pinimg.com/736x/52/59/8d/52598de7e6a3f345a4cf675398e23956.jpg"
                        alt="Media consumption playlist">
                     <class="playlist-title">
                       <h3>side quests </h3>
                    <p class="playlist-description">
                        i do draw, write, like to sing, edit UI/UX interfaces, daydream 24/7
                        <b>
                    </p>
              </article>
            </div>
        </section>
    </main>
</body>
</html>
