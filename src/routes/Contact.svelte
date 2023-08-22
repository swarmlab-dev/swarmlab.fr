<script>
    import MdEmail from 'svelte-icons/md/MdEmail.svelte'
</script>

<a class="anchor" id="anchor-contact"> </a>
<div class="hero">
    <h2>Want to know more about our expertise?</h2>
    <div class="container">
        <a href="mailto:contact@swarmlab.fr">
            <div class="button">
                <div class="icon">
                    <MdEmail/>
                </div>
                <p class="mail">contact@swarmlab.fr</p>
            </div>
        </a>
    </div>
</div>

<style>
    .hero {
        background: linear-gradient(white, var(--secondary-color));
        padding: 5em 0;
        color: white;
    }
    .button {
        width: 30rem;
        height: 4.8rem;
        border: none;
        background: #ffffff;
        border-radius: 1.5rem;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 0.875rem;
        margin: 0rem auto;
    }
    .mail {
        font-weight: 400;
        font-size: 1.5rem;
        vertical-align: middle;
    }
    .icon {
      width: 32px;
      height: 32px;
    }
    a {
        text-decoration: none;
    }

    .button {
        transition: 0.5s;
        cursor: pointer;
        color: var(--primary-color);
    }

    .button:hover {
        transition: 0.5s;
        animation: glow 2s linear infinite;
        -webkit-box-shadow:0px 0px 15px 4px rgba(45,255,196,0.9);
        -moz-box-shadow: 0px 0px 15px 4px rgba(45,255,196,0.9);
        box-shadow: 0px 0px 10px 4px rgba(45,255,196,0.9);
    }
    .button:active {
        transition: 0s;
        background-image: linear-gradient( 89.7deg, rgb(7, 197, 211) 2.7%, rgb(236, 193, 50) 92.4% );
        color: white;
    }

    @keyframes glow {
        0% {
            filter: hue-rotate(10deg);
        }

        100% {
            filter: hue-rotate(360deg);
        }
    }


</style>