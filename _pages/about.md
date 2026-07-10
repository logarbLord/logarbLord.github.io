---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## About me
Hello, I am an online digital artist. I mostly make tarkov mods/assets, but sometimes I'll dip into other ventures (such as this website) to test my skills and conviction. This website is to catalogue my art/creative ventures. Feel free to explore!

### Associates
I currently hang out with the [WTT team](https://www.welcometotarkov.com/). They are a huge help in learning both asset creation and tarkov modding.
<br />Their [Discord](https://discord.com/invite/welcometotarkov)

<p align="center">
    <a href="RandomSong" onclick="randomRedirect(event)">
        <img    src="/images/cooltextFlamingMusic.gif"
                alt="Music gif, random redirect when clicked."
                width="500">
    </a>
</p>
<script>
    function randomRedirect(event){
        event.preventDefault();
        const links = [
            /* King Gizzard & the Lizard Wizard - Level 5 */
                "https://www.youtube.com/watch?v=mp-HWukUDSE",
            /* xi - Blue Zenith */
                "https://www.youtube.com/watch?v=vatcanQQJvQ",
            /* Cymbals - ｢アメリカの女王｣ */
                "https://www.youtube.com/watch?v=UxMkQJDbUr8",
            /* Kasabian - You're In Love With a Psycho */
                "https://www.youtube.com/watch?v=kimPUWSwxIs",
            /* Kanye West - Flashing Lights (Alternate Intro) */
                "https://www.youtube.com/watch?v=O0Cw1SLdxxE",
            /* ABM - 'YARARARA' */
                "https://www.youtube.com/watch?v=T24rF_x0TmQ",
            /* Polyphia - CAN YOU FEEL IT */
                "https://www.youtube.com/watch?v=QB15JltRf-M",
            /* WSS Playground - きゅびずむ */
                "https://www.youtube.com/watch?v=N6DMXNyvAxs",
            /* WSS Playground - きゅびびびびずむ */
                "https://www.youtube.com/watch?v=DjGxGMxvg4M",
            /* Mai Yamane - Tasogare */
                "https://www.youtube.com/watch?v=IhCDK_pSjnk",
            /* 4:44 - JAY-Z (Feat. Tyler, the Creator and Hannah Williams & The Affirmations) */
                "https://www.youtube.com/watch?v=8pIhrMIsPAE",
            /* Гунеш - Ритмы Кавказа */
                "https://www.youtube.com/watch?v=VZ3cuw9cdI8",
            /* Massive Attack - Angel */
                "https://www.youtube.com/watch?v=hbe3CQamF8k",
            /* Kanye West - Mama's Boyfriend */
                "https://www.youtube.com/watch?v=fR1c8Qw3wEA",
            /* Crumb - Locket */
                "https://www.youtube.com/watch?v=BqnG_Ei35JE",
            /* Rob Cantor - I'M GONNA WIN */
                "https://www.youtube.com/watch?v=p_AY5pAAbQY",
            /* Vashti Bunyan - If I Were - Same But Different */
                "https://www.youtube.com/watch?v=6tz4xJWbY9s",
            /* UN Owen Was Her */
                "https://www.youtube.com/watch?v=8jJZA-O_B78",
            /* Gabbaheads - I'm A Thunderdome Baby */
                "https://www.youtube.com/watch?v=ifH7TDnyVm0",
            /* Technohead - I Wanna Be A Hippy */
                "https://www.youtube.com/watch?v=nmYi5u9BhtI",
            /* Erik Satie - Gnossienne in Asia Minor. interpreted by Forgotten Fish Memory Orchestra */
                "https://www.youtube.com/watch?v=_iaGcdlWk6k",
            /* The Chemical Brothers - Go */
                "https://www.youtube.com/watch?v=LO2RPDZkY88"
        ];
        window.location.href = 
            links[Math.floor(Math.random() * links.length)];
        /*
            math.random (random number between 0.0 and 1.0)
            links.length (gets number of items in array (links))
            math.floor (rounds down. it needs a whole number)
            so this multiplies a random value (0.0-1.0), then multiplies it by the amount of items in the array, and rounds down. then redirects to that number page.
        */
    }
</script>