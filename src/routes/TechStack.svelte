<script>
    import bitcoin from "$lib/assets/bitcoin.png"
    import polkadot from "$lib/assets/polkadot.png"
    import stellar from "$lib/assets/stellar.png"
    import polygon from "$lib/assets/polygon.png"
    import ethereum from "$lib/assets/ethereum.png"
    import solidity from "$lib/assets/solidity.png"
    import ipfs from "$lib/assets/ipfs.png"
    import web3 from "$lib/assets/web3.png"

    const list = [
        {
            alt: "bitcoin",
            url: bitcoin,
        },
        {
            alt: "stellar",
            url: stellar,
        },
        {
            alt: "polkadot",
            url: polkadot
        },
        {
            alt: "polygon",
            url: polygon
        },
        {
            alt: "ethereum",
            url: ethereum
        },
        {
            alt: "solidity",
            url: solidity
        },
        {
            alt: "ipfs",
            url: ipfs
        },
        {
            alt: "web3",
            url: web3
        }
    ]
</script>

<div id="infinite" class="highway-slider">
    <div class="highway-barrier">
        <ul class="highway-lane">
        {#each list as {alt,url}}
            <li class="highway-car">
                <img src={url} alt={alt} />
            </li>
        {/each}
        {#each list as {alt,url}}
            <li class="highway-car">
                <img src={url} alt={alt} />
            </li>
        {/each}
        </ul>
    </div>
</div>

<style>
    ul {
        list-style-type: none;
        
    }
    li {
        float: left;
        margin-right: 10em;
    }
    img {
        height: 40px;
        filter: grayscale(20)
    }
    
    div.highway-slider {
        display:flex;
        justify-content:center;
        width:100%;
        height:150px;
    }
    div.highway-barrier {
        overflow:hidden;
        position:relative;
    }
    ul.highway-lane {
        display:flex;
        height:100%;
        width:500%;
    }
    li.highway-car {
        flex:1;
        display:flex;
        justify-content:center;
        align-items:center;
        background:#fff;
        color:#343434;
        width:180px;
        animation:translateinfinite 20s linear infinite;
    }
    img:hover{
        -o-transition:.2s;
        -ms-transition:.2s;
        -moz-transition:.2s;
        -webkit-transition:.2s;
        transition:.2s;
        filter: grayscale(0)
    }
    
    @keyframes translateinfinite {
        100% { transform:translateX(calc(-180px * 12));  }
    }
    #infinite div.highway-barrier {
        background:#fff;
        &::before,
        &::after {
            content: " ";
            position:absolute;
            z-index:9;
            width:180px;
            height:100%;	
        }
        &::before {
            top:0;left:0;
            background: linear-gradient(to right, rgba(255,255,255,1) 0%, rgba(255,255,255,0) 100%);
        }
        &::after {
            top:0;right:0;
            background: linear-gradient(to left, rgba(255,255,255,1) 0%, rgba(255,255,255,0) 100%);
        }
    }
    #infinite ul.highway-lane {
        width:calc(180px * 24);
    }


</style>