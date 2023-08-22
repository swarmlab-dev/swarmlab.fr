<script>
    import lucien from "$lib/assets/lucien.jpeg";
</script>

<a class="anchor" id="anchor-who"> </a>
<h2>About</h2>
<div class="container">
    <div class="grid">
        <div  class="image">
            <div class="avatar" style="background-image: url({lucien})"/>
            <p class="name">Lucien Loiseau</p>
        </div>
        <div class="who">
            <p>
                Lucien is a creative mind with a passion for using technology to connect people, devices and places. With over a decade of experience, 
                he woven his innovative spirit into diverse projects. As Director of Network & Services at Nodle, he architected the first incentivized 
                wireless IoT network, pioneering blockchain integration and fostering technical evolution. Lucien co-founded Coalition Network, shaping a 
                privacy-first contact tracing app combating COVID-19. At RightMesh, he led mesh networking innovation contributing to global standards.   
                His academic journey, including a Ph.D. in System and Telecommunication, reflects his dedication to cutting-edge research. 
                Let's collaborate and bring your tech dreams to life!
            </p>
        </div>
    </div>
</div>

<style>
    .grid {
        display: grid;
        grid-template-columns: repeat(10, 1fr);
        gap: 3em;
    }
    .who {
        grid-column: span 7;
    }
    p {
        color: var(--secondary-color);
        font-size: 1.1em;
        line-height: 1.6;
        text-align: justify;
    }
    .image {
        grid-column: span 3;        
        text-align: center;
        margin:auto;
    }
    .name {
        color: var(--secondary-color);
    }
    .avatar {
        width: 120px;
        height: 120px;
        background-size: contain;
        border-radius: 50%;
        box-shadow: 10px 10px 10px #ccc;
        -moz-box-shadow: 10px 10px 10px #ccc;
        -webkit-box-shadow: 10px 10px 10px #ccc;
        -khtml-box-shadow: 10px 10px 10px #ccc;
    }
</style>