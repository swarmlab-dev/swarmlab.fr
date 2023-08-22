<script>
    import nodle from "$lib/assets/nodle.png"
    import coalition from "$lib/assets/coalition.png"
    import rightmesh from "$lib/assets/rightmesh.jpg"
    import blockchainsociete from "$lib/assets/blockchainsociete.png"
    import symbiosis from "$lib/assets/symbiosis.png"

    const list = [
        {
            alt: "nodle",
            logo: nodle,
            url: "https://nodle.com"
        },
        {
            alt: "coalition",
            logo: coalition,
            url: "https://coalitionnetwork.org/"
        },
        {
            alt: "rightmesh",
            logo: rightmesh,
            url: "https://rightmesh.io"
        },
        {
            alt: "blockchain & societe",
            logo: blockchainsociete,
            url: "https://blockchainsociete.org/"
        },
        {
            alt: "symbiosis",
            logo: symbiosis,
            url: "https://symbiosis.metapixel.art/"
        },
    ]
</script>

<div class="container" id="anchor-partners">
    <ul class="grid">
        {#each list as {alt,logo,url}}
            <li class="item">
                <a href={url}  target="_blank"><img src={logo} alt={alt} /></a>
            </li>
        {/each}
    </ul>
</div>

<style>
    ul {
        display: flex;
        padding-inline-start: 0px;
        width: 100%;
        list-style: none;
    }
    ul li {
        flex-grow:2;
        padding-right:30px;
        text-align:center;
        filter: grayscale(20)
    }
    img {
        height: 40px;
    }
    li:hover{
        -o-transition:.2s;
        -ms-transition:.2s;
        -moz-transition:.2s;
        -webkit-transition:.2s;
        transition:.2s;
        filter: grayscale(0)
    }
</style>