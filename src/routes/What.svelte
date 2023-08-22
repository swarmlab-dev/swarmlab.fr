<script>
    import RainbowButton from "$lib/RainbowButton.svelte";
    import stock from "$lib/assets/stock.jpg";
    import MdMailOutline from 'svelte-icons/md/MdMailOutline.svelte'
</script>

<a class="anchor" id="anchor-what"> </a>
<h2>Our Mission</h2>
<div class="container">
    <div class="grid">
        <div class="what">
            <p>
                Our mission is to accelerate the digital transformation of connecting people through technology. The Internet laid
                a common infrastructure for communication on top of which crypto and blockchain technology are building the common
                infrastructure for finance. By encoding ownership and financial primitive right into the web, we can deeply redesign 
                how Internet users interacts and share value. If you are building a crypto/web3 project, chances are that we can help you! 
                <br/><br/>
                Contact us to know more about what we do!
            </p>

            <RainbowButton>
                <span class="icon"><MdMailOutline/></span>
                <span class="button-text">Contact Us</span>
            </RainbowButton>
        </div>
        <div  class="image" style="background-image: url({stock});">
        </div>
    </div>
</div>

<style>
    span.icon {
        float: left;
        width: 20px;
        height: 20px;
        margin-right: 0.3em;
    }
    span.button-text {
        vertical-align: middle;
    }
    .grid {
        display: grid;
        grid-template-columns: repeat(12, 1fr);
        gap: 3em;
    }
    .what {
        grid-column: span 6;
    }
    p {
        color: var(--secondary-color);
        font-size: 1.1em;
        line-height: 1.6;
        text-align: justify;
        text-justify: inter-word;
    }
    .image {
        grid-column: span 6;
        background-size: cover;
        border-radius: 0.5em;
        box-shadow: 10px 10px 10px #ccc;
        -moz-box-shadow: 10px 10px 10px #ccc;
        -webkit-box-shadow: 10px 10px 10px #ccc;
        -khtml-box-shadow: 10px 10px 10px #ccc;
    }
</style>