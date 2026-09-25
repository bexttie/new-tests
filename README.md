# new-tests

<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>aweelou | profile</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,500;1,400&display=swap" rel="stylesheet">

    <style>

        /* =========================================
           RESET
        ========================================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {

            background: #000000;

            color: #d6cecc;

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

            margin-bottom: 24px;

        }


        .profile-avatar {

            width: 92px;

            height: 92px;

            flex-shrink: 0;

            border-radius: 50%;

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

            font-family: Georgia, 'Times New Roman', serif;

            font-size: 21px;

            font-weight: bold;

            color: #e8dfdc;

            line-height: 1.3;

        }


        .profile-name .dot {

            color: #c8beba;

        }


        .profile-handle {

            font-family: Arial, Helvetica, sans-serif;

            font-size: 18px;

            font-weight: normal;

            color: #8b817f;

        }


        .profile-description {

            margin-top: 10px;

            font-family: Arial, Helvetica, sans-serif;

            font-size: 13px;

            line-height: 1.45;

            color: #d6cecc;

        }


        .profile-description a {

            text-decoration: underline;

            text-underline-offset: 2px;

        }


        .profile-note {

            color: #8b817f;

            font-size: 11px;

            margin-top: 2px;

        }


        /* =========================================
           BUTTONS
        ========================================= */

        .profile-actions {

            display: flex;

            gap: 10px;

            margin-bottom: 16px;

        }


        .action-button {

            width: 80px;

            height: 37px;

            border: none;

            border-radius: 0;

            background: #d8cecb;

            color: #171313;

            font-size: 14px;

            font-weight: normal;

            text-align: center;

            display: flex;

            align-items: center;

            justify-content: center;

        }


        .action-button:hover {

            background: #bdb1ad;

            text-decoration: none;

        }


        /* =========================================
           TWO COLUMN CONTENT
        ========================================= */

        .content-grid {

            display: grid;

            grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);

            gap: 16px;

            align-items: start;

        }


        .left-column,

        .right-column {

            min-width: 0;

        }


        /* =========================================
           PROFILE TEXT BOXES
        ========================================= */

        .text-box {

            border: 1px solid #d6cecc;

            padding: 7px 8px;

            margin-bottom: 10px;

            color: #d6cecc;

            font-family: Arial, Helvetica, sans-serif;

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


        /* =========================================
           FRIEND ACTIVITY
        ========================================= */

        .section-title {

            font-family: Georgia, 'Times New Roman', serif;

            font-size: 19px;

            font-weight: normal;

            line-height: 1.2;

            color: #d6cecc;

            margin-bottom: 10px;

        }


        .section-line {

            width: 100%;

            height: 2px;

            background: #9a8c89;

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

            border-radius: 50%;

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

            color: #d6cecc;

            margin-bottom: 2px;

        }


        .friend-details {

            font-size: 11px;

            line-height: 1.3;

            color: #c4b9b5;

            overflow-wrap: anywhere;

        }


        .friend-details .muted {

            color: #8b817f;

        }


        /* =========================================
           PLAYLISTS
        ========================================= */

        .playlists {

            margin-top: 12px;

        }


        .playlist-header {

            font-family: Georgia, 'Times New Roman', serif;

            font-size: 19px;

            font-weight: normal;

            color: #d6cecc;

            margin-bottom: 8px;

        }


        .playlist-line {

            width: 100%;

            height: 3px;

            background: #9a8c89;

            margin-bottom: 8px;

        }


        .playlist-grid {

            display: grid;

            grid-template-columns: repeat(3, minmax(0, 1fr));

            gap: 8px;

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

            color: #d6cecc;

        }


        .playlist-description {

            margin-top: 7px;

            font-size: 11px;

            line-height: 1.4;

            color: #b8aaa6;

        }


        /* =========================================
           RESPONSIVE
        ========================================= */

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


        <!-- =====================================
             PROFILE
        ====================================== -->

        <header class="profile">


            <div class="profile-avatar">

                <img src="#" alt="Profile picture">

            </div>


            <div class="profile-info">


                <h1 class="profile-name">

                    aweelou <span class="dot">·</span> sketch

                    <span class="profile-handle">@aweelou</span>

                </h1>


                <div class="profile-description">

                    they 21 unlabeled white eng/fr

                    <br>

                    <a href="#">main</a>

                    <a href="#">ao3</a>

                    <a href="#">priv</a>

                    <a href="#">spotify</a>

                    <a href="#">carrd</a>

                </div>


                <p class="profile-note">

                    pls avoid gendered terms &lt;3

                </p>


            </div>


        </header>



        <!-- =====================================
             BUTTONS
        ====================================== -->

        <div class="profile-actions">


            <a href="#" class="action-button">

                Follow

            </a>


            <a href="#" class="action-button">

                Message

            </a>


        </div>



        <!-- =====================================
             TWO COLUMNS
        ====================================== -->

        <div class="content-grid">



            <!-- =================================
                 LEFT COLUMN
            ================================== -->

            <section class="left-column">



                <div class="text-box">


                    <p>

                        before you follow i cuss a lot,

                        i go on fanart or pic account rt

                        sprees and regular lyrics

                        spams, rpf/rps, occasional

                        nsfw (nothing explicit w/o

                        tags)

                    </p>


                </div>



                <div class="text-box">


                    <p>

                        i won't fb if we don't have

                        ults in common, u participate

                        in fanwars or bringing negative

                        to the tl or anti-multi, too rt

                        heavy/no interaction, u were

                        born before '94 / after '06, no

                        carrd or basic info in profile

                        (im kinda selective)

                    </p>


                </div>



            </section>



            <!-- =================================
                 RIGHT COLUMN
            ================================== -->

            <section class="right-column">


                <h2 class="section-title">

                    Friend Activity

                </h2>


                <div class="section-line"></div>


                <div class="friend-list">



                    <!-- FRIEND 1 -->

                    <article class="friend">


                        <div class="friend-avatar">

                            <img src="#" alt="Friend avatar">

                        </div>


                        <div class="friend-info">


                            <p class="friend-name">

                                jiung

                            </p>


                            <p class="friend-details">

                                Nerves

                                <br>

                                DPR IAN

                                <br>

                                <span class="muted">

                                    ♫ Moodswings in...

                                </span>

                            </p>


                        </div>


                    </article>



                    <!-- FRIEND 2 -->

                    <article class="friend">


                        <div class="friend-avatar">

                            <img src="#" alt="Friend avatar">

                        </div>


                        <div class="friend-info">


                            <p class="friend-name">

                                gaon

                            </p>


                            <p class="friend-details">

                                haaAkkKKK!!

                                <br>

                                OurR

                                <br>

                                <span class="muted">

                                    ♫ haAaAkKKK!!!

                                </span>

                            </p>


                        </div>


                    </article>



                    <!-- FRIEND 3 -->

                    <article class="friend">


                        <div class="friend-avatar">

                            <img src="#" alt="Friend avatar">

                        </div>


                        <div class="friend-info">


                            <p class="friend-name">

                                yeonjun

                            </p>


                            <p class="friend-details">

                                Last Day On Earth

                                <br>

                                beabadoobee

                                <br>

                                <span class="muted">

                                    ♫ Our Extended P...

                                </span>

                            </p>


                        </div>


                    </article>



                </div>


            </section>



        </div>



        <!-- =====================================
             PUBLIC PLAYLISTS
        ====================================== -->

        <section class="playlists">


            <h2 class="playlist-header">

                Public Playlists

            </h2>


            <div class="playlist-line"></div>


            <div class="playlist-grid">



                <!-- PLAYLIST 1 -->

                <article class="playlist-card">


                    <img
                        class="playlist-image"
                        src="#"
                        alt="Love zone playlist"
                    >


                    <h3 class="playlist-title">

                        love zone

                    </h3>


                    <p class="playlist-description">

                        SVT hoshi dino the8

                        <br>

                        scoups seungkwan

                    </p>


                </article>



                <!-- PLAYLIST 2 -->

                <article class="playlist-card">


                    <img
                        class="playlist-image"
                        src="#"
                        alt="Mmmmmhm playlist"
                    >


                    <h3 class="playlist-title">

                        mmmmmhm ?

                    </h3>


                    <p class="playlist-description">

                        ( ˶ˆᗜˆ˵ ) h. cats,

                        <br>

                        writing, art, the sea,

                    </p>


                </article>



                <!-- PLAYLIST 3 -->

                <article class="playlist-card">


                    <img
                        class="playlist-image"
                        src="#"
                        alt="Media consumption playlist"
                    >


                    <h3 class="playlist-title">

                        media consumption

                    </h3>


                    <p class="playlist-description">

                        just to Feel Smth

                        <br>

                        BOOKS pjo soc TV

                    </p>


                </article>



            </div>


        </section>



    </main>


</body>

</html>
