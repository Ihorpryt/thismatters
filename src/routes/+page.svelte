<script>
    import './styles.css';
</script>

<div class="content">

    <div class="menu">

        <div class="img-wrapper">
            <img class="logo" src="https://thismatters.agency/wp-content/uploads/2023/03/thismatters-logo.svg" alt="logo" /> 
        </div>
        <ul>
            <li>Home</li>
            <li>Entwicklung</li>
            <li>Content</li>
            <li>SEO</li>
            <li>Hosting</li>
            <li>Blog</li>
            <li>About Us</li>
        </ul>
        <div class="btn-wrapper">
            <div class="btn-small">Kontakt</div>
         </div>
    </div>

    
    <div class="iframe">
        <spline-viewer url="https://prod.spline.design/MuZEsEJvvXlaJmd5/scene.splinecode"></spline-viewer>
    </div>

    <div class=text-info>
        <h3>Hmmm, that page doesn't exist</h3>
        <p>Head over to our homepage that definitely exists</p>
        <a href="#">
        <div class="btn">Back to Home</div>
        </a>
    </div>

</div>




<style>
    .content{
        font-family: 'Inter', sans-serif;
        height: 100vh;
        width: 100vw;
        background-image: url(https://thismatters.agency/cdn-cgi/image/quality=90,gravity=auto,sharpen=1,metadata=none,format=auto,onerror=redirect/wp-content/uploads/2023/08/pattern.svg);
    background-position: left top;

        background-color: #F4F6F9;
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;
        /* justify-content: center; */
    }
    .iframe {

        width: 100%;
        height: 100%;
        position: absolute;
        z-index: 1;
    }
    .menu {
        display: flex;
        justify-content: space-evenly;
        align-items: center;

        max-width: 1214px;
        height: 92px;
        width: 100%;
        
    }
    .img-wrapper {

        width: 100%;
        /* flex-basis: 97%; */
    }
    ul {
        margin: 0;
        padding: 0;
        display: flex;
        gap: 24px;
        justify-content: center;
        align-items: center;
        text-align: center;
    }
    li {
        display: block;
        font-family: Inter;
        font-size: 14px;
        font-weight: 500;
        width: max-content;
    }
    .logo {
        width: 180px;
    }
    .btn-wrapper {
        display: flex;
        width: 100%;
        justify-content: flex-end;
    }
    .btn-small {
        padding: 5px 16px;
        background-color: #622AFF;
        border-radius: 100px;
        color: white;
        font-size: 14px;
        font-style: normal;
        font-weight: 500;
        line-height: 22px; 
    }
    .text-info {
        margin-top: 400px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
    }
    h3 {
        color: #364153;

        margin: 0;
        margin-bottom: 16px;
        font-size: 26px;
        font-style: normal;
        font-weight: 500;
        line-height: 120%; 
        letter-spacing: -1.04px;
    }
    p {
        color: #364153;
        margin: 0;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: 28px; /* 155.556% */
        letter-spacing: -0.18px;
    }
    .btn {
        color: #060B13;
        box-sizing: border-box;
        margin-top: 48px;
        font-size: 22px;
        font-family: Inter, sans-serif;
        font-weight: 400;
        padding: 14px 36px;
        /* width: fit-content; */
        position: relative;
        z-index: 3;

    }
    .btn:hover {
        color:#622AFF;
    }
    .btn::before {
        content: "";
        position: absolute;
        inset: 0;
        border-radius: 50px; 
        padding: 2px; 
        background:linear-gradient(45deg,#EE787A,#DD04D1,#622AFF); 
        -webkit-mask: 
            linear-gradient(#fff 0 0) content-box, 
            linear-gradient(#fff 0 0);
        -webkit-mask-composite: xor;
          mask-composite: exclude; 
    }

    @media only screen and (max-width: 600px) {
        .iframe {
            top: -48px;
        }
    .logo {
        margin-left: 16px;
    }
    .btn-small {
        margin-right: 16px;
    }
    ul {
        display: none;    
    }
    .text-info {
        margin-top: 375px;
        padding: 0 16px;
    }
    
}
</style>