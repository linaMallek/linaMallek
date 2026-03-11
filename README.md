<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lina Mallek · GitHub profile</title>
    <!-- No external styles — all embedded for a clean, portable markdown vibe -->
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background: linear-gradient(145deg, #0a0c10 0%, #161b22 100%);
            font-family: 'Segoe UI', Roboto, system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
            display: flex;
            justify-content: center;
            padding: 2rem 1rem;
            color: #e6edf3;
        }
        .card {
            max-width: 1000px;
            width: 100%;
            background: rgba(13, 17, 23, 0.85);
            backdrop-filter: blur(4px);
            border-radius: 3rem 3rem 2rem 2rem;
            box-shadow: 0 30px 50px rgba(0,0,0,0.7), 0 0 0 1px #3d444d inset;
            overflow: hidden;
            padding: 2rem 2.2rem 2.5rem;
            border: 1px solid rgba(70, 130, 200, 0.2);
        }
        h1 {
            font-size: 3.2rem;
            font-weight: 700;
            letter-spacing: 1px;
            background: linear-gradient(130deg, #9f7aea, #63b3ed, #4fd1c5);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 0.25rem;
            text-shadow: 0 0 15px #7aa2f7;
        }
        h3 {
            font-weight: 400;
            font-size: 1.5rem;
            background: linear-gradient(120deg, #c0caf5, #a9b8e8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 0.75rem;
            border-bottom: 1px dashed #2a3a4a;
            padding-bottom: 0.8rem;
            display: inline-block;
        }
        .tagline {
            font-size: 1.2rem;
            color: #b3c7e5;
            max-width: 700px;
            margin: 0.5rem auto 1.5rem auto;
            background: #1e2633;
            padding: 0.5rem 1.8rem;
            border-radius: 60px;
            border-left: 5px solid #58a6ff;
            box-shadow: 0 8px 16px -8px #030409;
        }
        .banner {
            width: 100%;
            border-radius: 32px;
            margin: 1.8rem 0 2rem 0;
            box-shadow: 0 20px 30px -10px black, 0 0 0 2px #2f3d4e inset;
            transition: transform 0.3s ease;
        }
        .banner:hover {
            transform: scale(1.01);
        }
        .section-title {
            font-size: 2rem;
            font-weight: 600;
            margin: 2rem 0 1.2rem 0;
            background: linear-gradient(135deg, #bb9af7, #7dcfff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .section-title::before {
            content: "⚡";
            font-size: 2.2rem;
            background: none;
            -webkit-text-fill-color: #f0b3e3;
        }
        .email-badge {
            margin: 1.5rem 0 0.5rem;
        }
        .email-badge a {
            background: #212c3a;
            padding: 0.7rem 2rem;
            border-radius: 50px;
            font-size: 1.25rem;
            font-weight: 500;
            color: #d9e6f2;
            text-decoration: none;
            border: 1px solid #3c5a7d;
            box-shadow: 0 5px 0 #0a121c;
            transition: 0.15s;
            display: inline-block;
        }
        .email-badge a:hover {
            background: #2d4055;
            border-color: #6494cc;
            transform: translateY(-3px);
            box-shadow: 0 8px 0 #0a121c;
        }
        .toolkit {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem 1.5rem;
            justify-content: center;
            background: rgba(0, 20, 40, 0.4);
            padding: 2rem 1.5rem;
            border-radius: 60px;
            margin: 1.8rem 0;
            border: 1px solid #2d4055;
            backdrop-filter: blur(4px);
        }
        .toolkit img {
            width: 48px;
            height: 48px;
            filter: drop-shadow(0 4px 6px #070b10);
            transition: 0.2s;
            background: #10161e;
            border-radius: 14px;
            padding: 6px;
            border: 1px solid #395979;
        }
        .toolkit img:hover {
            transform: translateY(-6px) scale(1.1);
            filter: drop-shadow(0 12px 10px #1e3447);
            background: #1a2633;
            border-color: #7799cc;
        }
        .stats-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            gap: 2rem;
            margin: 2.5rem 0 1.5rem;
        }
        .stat-item {
            background: #0d1420;
            border-radius: 32px;
            padding: 0.5rem;
            border: 1px solid #3b4b62;
            box-shadow: 0 15px 20px -10px #02060a;
            transition: 0.2s;
        }
        .stat-item:hover {
            border-color: #8bacd9;
            box-shadow: 0 0 20px #1f496b;
        }
        .stat-item img {
            display: block;
            border-radius: 24px;
            max-width: 100%;
            height: auto;
        }
        .profile-views {
            margin-top: 2rem;
            font-size: 1.4rem;
            display: flex;
            justify-content: center;
        }
        .views-badge {
            background: #18222f;
            padding: 0.5rem 1.8rem;
            border-radius: 60px;
            border: 1px solid #4f6b8a;
            color: #bdd4f0;
            font-weight: 500;
            box-shadow: 0 0 12px #2d4b70;
        }
        .views-badge img {
            vertical-align: middle;
            margin-right: 8px;
            width: 24px;
            border-radius: 0;
            background: transparent;
        }
        .footer-note {
            margin-top: 3.2rem;
            padding-top: 1.5rem;
            text-align: center;
            border-top: 2px dashed #2b3f56;
            font-size: 1.5rem;
            font-weight: 400;
            color: #aac3e0;
            text-shadow: 0 2px 5px #02060a;
            letter-spacing: 0.5px;
        }
        .footer-note span {
            display: inline-block;
            animation: float 3s infinite ease-in-out;
        }
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-5px); }
            100% { transform: translateY(0px); }
        }
        hr {
            border: 1px solid #26384b;
            margin: 2rem 0 1rem;
        }
        /* fix any misalignments */
        .center {
            text-align: center;
        }
        .glow {
            color: #d9e3f0;
        }
    </style>
</head>
<body>
    <div class="card">

        <!-- HEADER with proper name and title -->
        <div class="center">
            <h1>✨ Lina MALLEK ✨</h1>
            <h3>🎓 Computer Vision Graduate  |  Developer & AI Artist 🎨</h3>
            <div class="tagline">
                🚀 Passionate about creating innovative, AI-driven solutions that bridge technology and design.
            </div>
        </div>

        <!-- BANNER image (corrected attribute, removed stray text) -->
        <img src="https://user-images.githubusercontent.com/74038190/241765440-80728820-e06b-4f96-9c9e-9df46f0cc0a5.gif" 
             class="banner" 
             alt="Animated coding banner with abstract tech design"
             title="code & create">

        <!-- WELCOME MESSAGE -->
        <div class="center" style="margin-top: 20px;">
            <span style="font-size: 2.2rem; background: #1f2a37; padding: 0.3rem 2rem; border-radius: 60px; border-left: 8px solid #e38cff;">👋 Welcome to my GitHub Profile!</span>
        </div>

        <!-- CONTACT BUTTON (email) -->
        <div class="center email-badge">
            <a href="mailto:linamlk23@gmail.com">
                <img src="https://img.shields.io/badge/Email-linamlk23@gmail.com-blue?style=flat-square&logo=gmail" 
                     alt="Email badge" 
                     style="width: auto; height: 30px; border-radius: 0; background: transparent; filter: none; display: inline; padding: 0;">
                <!-- shield.io image directly used, no extra nesting needed -->
            </a>
        </div>

        <!-- ABOUT ME SECTION -->
        <div class="section-title">🚀 About Me</div>
        <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.2rem 2rem; background: #0f1621; padding: 1.8rem; border-radius: 48px; border: 1px solid #253649;">
            <div style="font-size: 1.3rem;">👋 <strong>Hi, I’m Lina Mallek</strong> — a passionate <span style="color:#b1e3ff;">Developer</span>, <span style="color:#d0bfff;">Designer</span> and <span style="color:#b1f0d6;">Computer Vision Engineer</span>.</div>
            <div style="font-size: 1.3rem;">🌱 <strong>Currently Learning:</strong> Python & Artificial Intelligence.</div>
            <div style="font-size: 1.3rem;">🎨 <strong>Skills:</strong> Image Analysis, Web Development, Computer Vision, and more!</div>
            <div style="font-size: 1.3rem;">👀 <strong>Interests:</strong> Coding, Hackathons, exploring innovative tech.</div>
        </div>

        <!-- TOOLS & LANGUAGES (all icons fixed, removed duplicates, added missing ones) -->
        <div class="section-title" style="margin-top: 3rem;">🛠️ Languages & Tools</div>
        <div class="toolkit">
            <!-- Python -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original-wordmark.svg" title="Python" alt="Python">
            <!-- Numpy -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-original.svg" title="NumPy" alt="NumPy">
            <!-- PyTorch -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/pytorch/pytorch-original.svg" title="PyTorch" alt="PyTorch">
            <!-- TensorFlow -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/tensorflow/tensorflow-original.svg" title="TensorFlow" alt="TensorFlow">
            <!-- Matplotlib -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/matplotlib/matplotlib-original.svg" title="Matplotlib" alt="Matplotlib">
            <!-- Streamlit -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/streamlit/streamlit-original.svg" title="Streamlit" alt="Streamlit">
            <!-- Postman -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/postman/postman-original.svg" title="Postman" alt="Postman">
            <!-- Java -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/java/java-original-wordmark.svg" title="Java" alt="Java">
            <!-- CSS3 -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg" title="CSS3" alt="CSS">
            <!-- HTML5 -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="HTML5" alt="HTML">
            <!-- JavaScript -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="JavaScript" alt="JavaScript">
            <!-- Node.js -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original.svg" title="Node.js" alt="Node.js">
            <!-- Prisma (original icon) -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/prisma/prisma-original.svg" title="Prisma" alt="Prisma">
            <!-- MySQL -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" title="MySQL" alt="MySQL">
            <!-- Git -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/git/git-original-wordmark.svg" title="Git" alt="Git">
            <!-- Linux -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/linux/linux-original.svg" title="Linux" alt="Linux">
            <!-- Unity -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/unity/unity-original.svg" title="Unity" alt="Unity">
            <!-- Notion -->
            <img src="https://github.com/devicons/devicon/blob/master/icons/notion/notion-original.svg" title="Notion" alt="Notion">
        </div>

        <!-- STATS SECTION : My Stats with streak and top langs (corrected layouts + fixed links) -->
        <div class="section-title">🔥 My Stats</div>

        <!-- Profile views counter (original style, but modernized) -->
        <div class="profile-views">
            <div class="views-badge">
                <img src="https://komarev.com/ghpvc/?username=linaMallek&color=brightgreen&style=for-the-badge" 
                     alt="Profile views counter" 
                     style="width: auto; height: 30px; background: transparent; border-radius: 0;">
                <!-- using image from komarev directly, but we keep inline for simplicity; note: the img src returns a badge, fine -->
            </div>
        </div>

        <!-- stats table replaced with flex for modern look, but preserve streak + languages -->
        <div class="stats-grid">
            <!-- GitHub streak card (with fixed username case: linaMallek) -->
            <div class="stat-item">
                <img src="https://github-readme-streak-stats.herokuapp.com?user=linaMallek&theme=radical&background=0d1117&border=2e4055&stroke=5f8ab6&ring=79c0ff&fire=ff9f7c&currStreakNum=ffffff&sideNums=b7d3ff" 
                     alt="GitHub Streak" 
                     width="400">
            </div>
        </div>

        <!-- Top languages card (fixed alignment, added border) -->
        <div style="display: flex; justify-content: center; margin: 1.5rem 0 0.5rem;">
            <div class="stat-item" style="max-width: 400px;">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=linaMallek&layout=compact&theme=vision-friendly-dark&hide_border=true&bg_color=0d1117&title_color=9f9ff0&text_color=cbd5e8" 
                     alt="Top Languages" 
                     width="380">
            </div>
        </div>

        <!-- additional fun metrics - could add github stats but keep clean -->
        <div style="display: flex; gap: 1.5rem; justify-content: center; flex-wrap: wrap; margin: 2.5rem 0 1rem;">
            <img src="https://img.shields.io/badge/dynamic/json?color=blue&label=followers&query=followers&url=https%3A%2F%2Fapi.github.com%2Fusers%2FlinaMallek&style=for-the-badge&logo=github" alt="followers" style="border-radius: 30px;">
            <img src="https://img.shields.io/badge/dynamic/json?color=purple&label=stars&query=stars&url=https%3A%2F%2Fapi.github.com%2Fusers%2FlinaMallek&style=for-the-badge&logo=github" alt="stars" style="border-radius: 30px;">
        </div>

        <!-- HIDDEN comment preservation: original comment from your file is kept but invisible in design (as html comment) -->
        <!--
        <!--- linaMallek/linaMallek is a ✨ special ✨ repository because its `README.md` appears on GitHub profile.
        You can click Preview link to take a look at your changes.
        -->
        <!-- That comment is intentionally hidden, but retained for consistency. -->

        <!-- FOOTER with nice thank you -->
        <div class="footer-note">
            <span>✨ Thank you for visiting! Let's build amazing things together ✨</span>
        </div>

        <!-- small signature: corrected the 'states' -> stats and prettier already ;) -->
        <div style="text-align: center; margin-top: 1.8rem; opacity: 0.8; font-size: 1rem; color: #6f8ab1;">
            ⚡ corrected & prettified · with extra stats ⚡
        </div>
    </div>
</body>
</html>
