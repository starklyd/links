<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Charlie Stark | Official Links</title>
    <meta name="description" content="Official links for avant-garde electronic musician Charlie Stark. Music, Videos, Press, and Live Sets.">
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&family=Syncopate:wght@400;700&display=swap" rel="stylesheet">
    <!-- Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --bg-color: #050505;
            --text-main: #f0f0f0;
            --text-muted: #a0a0a0;
            --accent-primary: #8a2be2;
            --accent-glow: rgba(138, 43, 226, 0.4);
            --card-bg: rgba(25, 25, 25, 0.6);
            --card-border: rgba(255, 255, 255, 0.08);
            --font-headings: 'Syncopate', sans-serif;
            --font-body: 'Outfit', sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: var(--font-body);
            line-height: 1.5;
            overflow-x: hidden;
            background-image: 
                radial-gradient(circle at 15% 50%, rgba(138, 43, 226, 0.08), transparent 25%),
                radial-gradient(circle at 85% 30%, rgba(0, 191, 255, 0.08), transparent 25%);
        }

        /* Background Effects */
        .background-effects {
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            z-index: -1;
            pointer-events: none;
        }
        .glow-orb {
            position: absolute;
            border-radius: 50%;
            filter: blur(80px);
            opacity: 0.5;
        }
        .orb-1 {
            width: 400px; height: 400px;
            background: var(--accent-primary);
            top: -100px; left: -100px;
            animation: float 15s ease-in-out infinite alternate;
        }
        .orb-2 {
            width: 300px; height: 300px;
            background: #00bfff;
            bottom: -50px; right: -50px;
            animation: float 20s ease-in-out infinite alternate-reverse;
        }
        @keyframes float {
            0% { transform: translate(0, 0) scale(1); }
            100% { transform: translate(50px, 50px) scale(1.1); }
        }

        /* Container & Layout */
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 2rem 1rem;
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        /* Typography */
        h1, h2, h3 {
            font-family: var(--font-headings);
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        
        a {
            color: inherit;
            text-decoration: none;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 3rem 0;
            animation: fadeInDown 1s ease-out;
        }
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .profile-image-container {
            position: relative;
            width: 150px;
            height: 150px;
            margin: 0 auto 1.5rem;
        }
        .profile-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 50%;
            position: relative;
            z-index: 2;
            border: 2px solid var(--accent-primary);
        }
        .glow-ring {
            position: absolute;
            top: -5px; left: -5px; right: -5px; bottom: -5px;
            background: linear-gradient(45deg, var(--accent-primary), #00bfff);
            border-radius: 50%;
            z-index: 1;
            filter: blur(10px);
            opacity: 0.7;
            animation: pulseGlow 3s infinite alternate;
        }
        @keyframes pulseGlow {
            0% { opacity: 0.5; filter: blur(8px); }
            100% { opacity: 0.9; filter: blur(15px); }
        }

        .artist-name {
            font-size: 3rem;
            margin-bottom: 0.5rem;
            background: linear-gradient(to right, #fff, var(--text-muted));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 800;
        }
        .artist-bio {
            color: var(--text-muted);
            font-size: 1.1rem;
            max-width: 400px;
            margin: 0 auto;
        }

        /* Newsletter */
        .newsletter {
            text-align: center;
            padding: 2rem;
            border-radius: 16px;
            margin-bottom: 1rem;
        }
        .subscribe-form {
            display: flex;
            gap: 0.5rem;
            margin-top: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
        }
        .subscribe-form input {
            padding: 0.8rem 1.5rem;
            border-radius: 30px;
            border: 1px solid var(--card-border);
            background: rgba(0,0,0,0.5);
            color: #fff;
            flex-grow: 1;
            max-width: 300px;
            font-family: var(--font-body);
            outline: none;
            transition: border-color 0.3s;
        }
        .subscribe-form input:focus {
            border-color: var(--accent-primary);
        }
        .btn-primary {
            background: linear-gradient(45deg, var(--accent-primary), #6a1b9a);
            border: none;
            color: white;
            padding: 0.8rem 2rem;
            border-radius: 30px;
            font-family: var(--font-headings);
            font-size: 0.9rem;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px var(--accent-glow);
        }
        .form-status {
            margin-top: 1rem;
            color: #00ff88;
            font-size: 0.9rem;
            opacity: 0;
            transition: opacity 0.3s;
        }
        .form-status.visible { opacity: 1; }

        /* Bento Grid */
        .bento-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            grid-auto-rows: 200px;
            gap: 1.5rem;
        }

        .bento-card {
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 20px;
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(10px);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            transition: transform 0.3s ease, border-color 0.3s ease;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            padding: 1.5rem;
        }
        .bento-card:hover {
            transform: translateY(-5px);
            border-color: rgba(255,255,255,0.2);
        }

        .no-padding { padding: 0; }
        
        /* Grid spans */
        .bento-wide { grid-column: span 2; }
        @media (max-width: 600px) { .bento-wide { grid-column: span 1; } }
        .bento-tall { grid-row: span 2; justify-content: flex-start; }

        /* Icon & Text Styling */
        .bento-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        .accent-blue { color: #00bfff; }
        .accent-purple { color: #8a2be2; }
        .accent-red { color: #ff3366; }
        .accent-green { color: #1db954; }

        .bento-card h3 {
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
            z-index: 2;
        }
        .bento-card p {
            font-size: 0.9rem;
            color: var(--text-muted);
            z-index: 2;
        }

        /* Feature Card (Spotify Release) */
        .feature-card {
            justify-content: flex-end;
            padding-bottom: 2rem;
            text-align: left;
            align-items: flex-start;
        }
        .card-image-bg {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background-size: cover;
            background-position: center;
            opacity: 0.4;
            transition: opacity 0.3s, transform 0.5s;
            z-index: 0;
        }
        .feature-card:hover .card-image-bg {
            opacity: 0.6;
            transform: scale(1.05);
        }
        .card-content {
            position: relative;
            z-index: 2;
            width: 100%;
        }
        .new-badge {
            background: var(--accent-primary);
            color: white;
            padding: 0.2rem 0.6rem;
            border-radius: 4px;
            font-size: 0.7rem;
            font-weight: bold;
            text-transform: uppercase;
            margin-bottom: 0.5rem;
            display: inline-block;
        }
        .icon-indicator {
            position: absolute;
            bottom: 0; right: 0;
            color: #1db954; 
            font-size: 2rem;
        }

        /* iFrames */
        .iframe-wrapper {
            position: relative;
            width: 100%;
            height: 100%;
            overflow: hidden;
            display: flex;
            align-items: center;
            background: #000;
        }
        .iframe-wrapper iframe {
            width: 100%;
            height: 100%;
            border: none;
            position: absolute;
            top: 0; left: 0;
        }
        .iframe-container {
            width: 100%;
            flex-grow: 1;
            height: calc(100% - 40px);
        }
        .card-footer-link {
            width: 100%;
            background: rgba(255,255,255,0.05);
            padding: 10px;
            font-size: 0.8rem;
            text-align: center;
            font-weight: bold;
            letter-spacing: 1px;
            border-top: 1px solid var(--card-border);
            transition: background 0.3s;
        }
        .card-footer-link:hover { background: rgba(255,255,255,0.1); }
        .sc-player-card { display: flex; flex-direction: column; justify-content: space-between; }


        /* Lists */
        .links-list-card {
            padding: 2rem;
            text-align: left;
            align-items: flex-start;
        }
        .list-title {
            font-size: 1rem;
            margin-bottom: 1.5rem;
            color: var(--accent-primary);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .clean-list {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 1rem;
            width: 100%;
        }
        .clean-list li a {
            display: block;
            padding: 0.8rem;
            background: rgba(0,0,0,0.3);
            border-radius: 8px;
            transition: background 0.2s, transform 0.2s;
            font-size: 0.95rem;
            border-left: 2px solid transparent;
        }
        .clean-list li a:hover {
            background: rgba(255,255,255,0.05);
            transform: translateX(5px);
            border-left-color: var(--accent-primary);
        }
        
        .press-list li a {
            display: flex;
            flex-direction: column;
            gap: 0.3rem;
        }
        .publication { font-weight: bold; color: #fff; font-size: 0.85rem;}
        .quote { color: var(--text-muted); font-style: italic; font-size: 0.8rem;}

        footer {
            text-align: center;
            padding: 2rem 0;
            color: var(--text-muted);
            font-size: 0.8rem;
            opacity: 0.6;
        }

    </style>
</head>
<body>
    <div class="background-effects">
        <div class="glow-orb orb-1"></div>
        <div class="glow-orb orb-2"></div>
    </div>

    <main class="container">
        <!-- Hero Section -->
        <header class="hero">
            <div class="profile-image-container">
                <!-- BASE64_IMG_HERO_PLACEHOLDER -->
                <img src="" id="hero-img" alt="Charlie Stark Portrait" class="profile-image">
                <div class="glow-ring"></div>
            </div>
            <h1 class="artist-name">Charlie<br>Stark</h1>
            <p class="artist-bio">Avant-garde electronic musician. "Grinding P Funk" meets Underground UK.</p>
        </header>

        <!-- Newsletter Section -->
        <section class="newsletter bento-card">
            <h2 class="list-title" style="margin-bottom:0.5rem;"><i class="fa-solid fa-envelope-open-text"></i> Join the Transmission</h2>
            <p style="font-size:0.9rem;">Exclusive updates on new music & secret gigs.</p>
            <form id="newsletter-form" class="subscribe-form">
                <input type="email" id="email-input" placeholder="Enter your email pulse..." required>
                <button type="submit" class="btn-primary">
                    <span class="btn-text">Connect</span>
                    <i class="fa-solid fa-bolt"></i>
                </button>
            </form>
            <div id="form-status" class="form-status">Transmission received. Welcome.</div>
        </section>

        <!-- Main Links (Bento Grid) -->
        <section class="bento-grid">

            <!-- Latest Release Spotlight -->
            <a href="https://open.spotify.com/album/4SQhQu68J8tCcIAgmMee2D" target="_blank" class="bento-card feature-card bento-wide" id="feature-card-bg">
                <!-- BASE64_IMG_LIVE_PLACEHOLDER below in data attr or css -->
                <div class="card-image-bg" id="live-img-bg"></div>
                <div class="card-content">
                    <span class="new-badge">Latest Release</span>
                    <h3>Another Lifetime</h3>
                    <p style="color:#ddd">Stream now on Spotify</p>
                    <div class="icon-indicator"><i class="fa-brands fa-spotify"></i></div>
                </div>
            </a>

            <!-- Ditto Link -->
            <a href="https://ditto.fm/strange-to-be-alive" target="_blank" class="bento-card">
                <i class="fa-solid fa-compact-disc bento-icon accent-blue"></i>
                <h3>Strange to Be<br>Alive</h3>
                <p>Listen via Ditto</p>
            </a>

            <!-- Bandcamp Embedded Player -->
            <div class="bento-card bento-tall no-padding">
                <div class="iframe-container">
                    <iframe style="border: 0; width: 100%; height: 100%;" src="https://bandcamp.com/EmbeddedPlayer/album=466503311/size=large/bgcol=333333/linkcol=0f91ff/tracklist=false/track=2567182898/transparent=true/" seamless></iframe>
                </div>
                <div class="card-footer-link">
                    <a href="https://charliestark.bandcamp.com/album/hallways-and-stairs" target="_blank">Buy 'Hallways and Stairs'</a>
                </div>
            </div>

            <!-- YouTube Video 1 -->
            <div class="bento-card bento-wide no-padding">
                <div class="iframe-wrapper">
                    <iframe src="https://www.youtube.com/embed/k3NoYtliyZY?si=n38Y5X0p-8MFHIFS" title="Charlie Stark Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>

            <!-- YouTube Video 2 -->
             <div class="bento-card bento-wide no-padding">
                <div class="iframe-wrapper">
                    <iframe src="https://www.youtube.com/embed/DVePcBAhW74?si=mCw6mfn6RbdE90Ij" title="Charlie Stark Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>

            <!-- Soundcloud Embedded Player UFO -->
            <div class="bento-card bento-wide no-padding sc-player-card">
                 <iframe width="100%" height="160" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/283373330&color=%237a28ff&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true"></iframe>
                 <div class="card-footer-link">
                    <a href="https://soundcloud.com/paradisescientist/charlie-stark-ufo-ep-radio-rip-world-premiere-hoxton-fm-normski" target="_blank">Hoxton FM exclusive with Dj Normski</a>
                </div>
            </div>

            <!-- Video 3: UFO 4K Video -->
            <div class="bento-card no-padding">
                <div class="iframe-wrapper">
                    <iframe src="https://www.youtube.com/embed/TAPfLYxE2pw" title="UFO 4K Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>

            <!-- Video 4: nseDuR6K8a4 -->
             <div class="bento-card no-padding">
                <div class="iframe-wrapper">
                    <iframe src="https://www.youtube.com/embed/nseDuR6K8a4?si=tBQi91plXxodR_FL" title="Charlie Stark Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>

            <!-- Charlie Stark ft Roots Manuva -->
             <a href="https://youtu.be/8jH_bSqv17s" target="_blank" class="bento-card">
                <i class="fa-brands fa-youtube bento-icon accent-red"></i>
                <h3>Ft Roots Manuva</h3>
                <p>Watch Link</p>
            </a>

            <!-- DJ Mixes & Aliases column -->
            <div class="bento-card bento-tall links-list-card">
                <h3 class="list-title"><i class="fa-solid fa-headphones"></i> Mixes & Aliases</h3>
                <ul class="clean-list">
                    <li><a href="https://soundcloud.com/paradisescientist/prologue-mix-forecast-mixtapes-reprezent-fm" target="_blank">Live Mix - Represent FM</a></li>
                    <li><a href="https://www.mixcloud.com/GlobalBeatsRadio/global-beats-radio-november-1st-2018-w-charlie-stark/" target="_blank">Live Mix - Global Beats Radio</a></li>
                    <li><a href="https://soundcloud.com/paradisescientist/ibeyi-oya-paradise-scientist-remix" target="_blank">Paradise Scientist (Alias)<br><span style="font-size:0.8rem;color:#888;">Ibeyi Oya Remix</span></a></li>
                </ul>
            </div>

            <!-- Press & Reviews List -->
            <div class="bento-card bento-tall links-list-card">
                <h3 class="list-title"><i class="fa-solid fa-newspaper"></i> Press & Reviews</h3>
                <ul class="clean-list press-list">
                    <li>
                        <a href="https://soundsoftheuniverse.com/product/ufo" target="_blank">
                            <span class="publication">Sound of the Universe</span>
                            <span class="quote">"Grinding P Funk"</span>
                        </a>
                    </li>
                    <li>
                        <a href="http://soundtraffic.pl/charlie-stark-ufo/" target="_blank">
                            <span class="publication">SoundTraffic Poland</span>
                            <span class="quote">UFO Review</span>
                        </a>
                    </li>
                    <li>
                        <a href="http://www.constantcircles.com/prem-sd002/" target="_blank">
                            <span class="publication">Constant Circles</span>
                            <span class="quote">Hallways and Stairs Premiere</span>
                        </a>
                    </li>
                    <li>
                        <a href="https://mixmag.net/read/infinite-machine-releases-debut-warsnare-album-warchestra-news/" target="_blank">
                            <span class="publication">Mixmag & Yahoo</span>
                            <span class="quote">Warchestra (Dan Samsa Collab)</span>
                        </a>
                    </li>
                </ul>
            </div>
            
        </section>

        <footer>
            <p>&copy; 2024 Charlie Stark. All Rights Reserved.</p>
        </footer>
    </main>

    <script>
        // Newsletter Form Handler
        document.getElementById('newsletter-form').addEventListener('submit', function(e) {
            e.preventDefault();
            const emailInput = document.getElementById('email-input');
            const statusDiv = document.getElementById('form-status');
            
            if (emailInput.value) {
                // Mock submission
                emailInput.value = '';
                statusDiv.classList.add('visible');
                setTimeout(() => {
                    statusDiv.classList.remove('visible');
                }, 4000);
            }
        });
    </script>
</body>
</html>
