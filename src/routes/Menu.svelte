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

<style>

.menu {
        display: flex;
        justify-content: space-evenly;
        align-items: center;

        max-width: 1214px;
        min-height: 92px;
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

    @media only screen and (max-width: 600px) {

    .logo {
        margin-left: 16px;
    }
    .btn-small {
        margin-right: 16px;
    }
    ul {
        display: none;    
    }

    }
</style>