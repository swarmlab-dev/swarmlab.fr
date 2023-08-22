
<a href="mailto:contact@swarmlab.fr">
    <div class="outer">
        <button>
            <slot />
        </button>
    </div>
</a>

<style>
    button {
        padding: 0.375em 0.5em;
        background-color: transparent;
        border: none;
        border-radius: 0.25em;
        color: white;
        font-size: 1em;
        cursor: pointer;
    }

    .outer {
        background-color: var(--primary-color);
        transition: 0.5s;
        width: fit-content;
        border: none;
        border-radius: 0.25em;
        position: relative;
    }

    .outer:hover {
        transition: 0.5s;
        animation: glow 2s linear infinite;
        -webkit-box-shadow:0px 0px 15px 4px rgba(45,255,196,0.9);
        -moz-box-shadow: 0px 0px 15px 4px rgba(45,255,196,0.9);
        box-shadow: 0px 0px 10px 4px rgba(45,255,196,0.9);
    }

    .outer:active {
        transition: 0s;
        background-image: linear-gradient( 89.7deg, rgb(7, 197, 211) 2.7%, rgb(236, 193, 50) 92.4% );
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