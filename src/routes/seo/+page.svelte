<script>
    import {onMount} from 'svelte';
    import lottie from 'lottie-web';

    import BtnLink from "../Btn-link.svelte";
    import Menu from "../Menu.svelte";
    import '../styles.css';


    let animationContainer

    onMount(() => {

        if (!animationContainer) return

        lottie.loadAnimation({
            container: animationContainer, 
            renderer: 'svg',
            loop: true,
            autoplay: true,
            path: 'src/routes/seo/SEO.json' 
        })

    })


</script>


<div class="content">

    <Menu />

    <div class=text-info>
        <div class="left-side">
        <p class="decor-text">Kategorie</p>
        <h2>SEO</h2>
        <p class="body-l">Suchmaschinenoptimierung (SEO) ist der Prozess der Verbesserung der Sichtbarkeit einer Website in den organischen Suchergebnissen von Suchmaschinen wie Google.</p>
        <p class="body-m">Entdecke mit "this:matters" die SEO-Agentur, die mehr als nur Rankings bietet. Unser Expertenteam bringt deine Marke durch massgeschneiderte Strategien an die Spitze.</p>
        <p class="body-m">Wir setzen auf nachhaltiges Wachstum, transparente Kommunikation und messbare Erfolge. Mit tiefgehendem Marktverständnis und einer zielgerichteten Herangehensweise verwandeln wir deine SEO-Ziele in sichtbare Ergebnisse.</p>
        <div class="btn-links"> 
            <BtnLink text="SEO Audit"/> 
            <BtnLink text="SEO Beratung"/>
            <BtnLink text="SEO Texte für Deinen Blog schreiben lassen"/>  
        </div>
        </div>
        <div class="right-side">
            <!-- <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script> -->
            <!-- <lottie-player src="src/routes/seo/SEO.json" background="transparent" speed="1" class="lottie" direction="1" mode="normal" loop autoplay></lottie-player> -->
            <!-- <lottie-player src={jsonData} background="transparent" speed="1" class="lottie" direction="1" mode="normal" loop autoplay></lottie-player> -->
            <div bind:this={animationContainer}></div>
        </div>
    </div>

    <div class="posts">
        <div class="post">
            <img class="post-image" src="https://thismatters.agency/wp-content/uploads/2023/11/Cloaking-Blogbeitrag-1536x878.jpg" alt="">
            <div class="copy">
                <h3>What is cloaking and how is it used in SEO?</h3>
                <p class="body-m">Cloaking, from English for “camouflage”, refers to a method in which different content is presented to search engines and users. This approach is used in the area of ​​SEO (Search Engine Optimization)...</p>
                <div class="writer">
                    <img class="avatar" src="https://thismatters.agency/wp-content/uploads/2023/03/Kevin-Kyburz-90x90.jpg" alt="">
                    <div class="writers-info">
                        <p class="accented-body-s">Kevin Kyburz</p>
                        <p class="body-s">24 August 2023</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="post">
            <img class="post-image" src="https://thismatters.agency/wp-content/uploads/2023/10/Interne-Links-SEO-Titelbild-1536x864.jpg" alt="">
            <div class="copy">
                <h3>Interne Links – Definition, Vorteile & Strategie</h3>
                <p class="body-m">Wenn es um die Optimierung deiner Website geht, sind interne Links ein Tool, das du nicht unterschätzen solltest. Sie bilden das unsichtbare Gerüst deiner Website, das sowohl Suchmaschinen ...</p>
                <div class="writer">
                    <img class="avatar" src="https://thismatters.agency/wp-content/uploads/2023/03/Kevin-Kyburz-90x90.jpg" alt="">
                    <div class="writers-info">
                        <p class="accented-body-s">Kevin Kyburz</p>
                        <p class="body-s">24 August 2023</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="post">
            <img class="post-image" src="https://thismatters.agency/wp-content/uploads/2023/10/SEO-Masnahmen-Titelbild-1536x864.jpg" alt="">
            <div class="copy">
                <h3>What is cloaking and how is it used in SEO?</h3>
                <p class="body-m">Cloaking, from English for “camouflage”, refers to a method in which different content is presented to search engines and users. This approach is used in the area of ​​SEO (Search Engine Optimization)...</p>
                <div class="writer">
                    <img class="avatar" src="https://thismatters.agency/wp-content/uploads/2023/03/Kevin-Kyburz-90x90.jpg" alt="">
                    <div class="writers-info">
                        <p class="accented-body-s">Kevin Kyburz</p>
                        <p class="body-s">24 August 2023</p>
                    </div>
                </div>
            </div>
        </div>

    </div>

</div>




<style>
    .content{
        font-family: 'Inter', sans-serif;
        -webkit-font-smoothing: antialiased;
        height: 100%;
        width: 100vw;
        background-image: url(https://thismatters.agency/cdn-cgi/image/quality=90,gravity=auto,sharpen=1,metadata=none,format=auto,onerror=redirect/wp-content/uploads/2023/08/pattern.svg);
        background-position: left top;

        background-color: #F4F6F9;
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;
        padding-bottom: 96px;
        /* justify-content: center; */
    }

    .lottie {
        width: 583px;
        height: 642px;
    }
    
    .text-info {
        margin-top:48px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        text-align: left;
        max-width: 1214px;
        width: 100%;
    }
    .left-side {
        display: flex;
        gap: 24px;
        flex-direction: column;
        width: 100%;
        padding: 0 16px;
    }
    .btn-links {
        display: flex;
        flex-direction: row;
        gap: 8px;
        flex-wrap: wrap;
    }
    .right-side  {
        width: 100%;
    }
    .posts {
        display: flex;
        flex-direction: column;
        gap: 48px;
        margin-top: 96px;
    }
    .post {
        display: flex;
        flex-direction: row;
        max-width: 1214px;
    }
    .post-image {
        width: 100%;
        background-color: aquamarine;
        border-radius: 48px;
        height: 366px;
    } 
    .copy {
        padding: 48px;
        display: flex;
        flex-direction: column;
        gap: 24px;
        justify-content: center;
    }
    .writer {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 12px;
    }
    .avatar {
        width: 48px;
        height: 48px;
        background-color: aquamarine;
        border-radius: 200px;
    }

    @media only screen and (max-width: 600px) {
        .text-info {
            flex-direction: column;
        }  
        .lottie {
        width: 100%;
        }
        .right-side {
            display: none;
        }
        .posts {
            padding: 0 16px;
        }
        .post {
        display: flex;
        flex-direction: column;
        max-width: 1214px;
        }
        .post-image {
            height: 230px;
        }
        .copy {
            padding: 48px 0;
        }
    }
</style>