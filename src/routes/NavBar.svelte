<script>
    import { page } from "$app/stores";
    import logo from "$lib/assets/logo-dark-line.png";

    const navs = [
        {
            title: "Home",
            href: "/"
        },
        {
            title: "Mission",
            href: "#anchor-what"
        },
        {
            title: "About",
            href: "#anchor-who"
        },
        {
            title: "Contact",
            href: "#anchor-contact"
        }
    ]

    $: routeId = $page.route.id;
</script>

<nav>
    <div class="container">
        <img src={logo} alt="SwarmLab"/>
        <ul>
            {#each navs as {title, href}}
                <li>
                    <a {href} class:active={routeId == href} title={title}>{title}</a>
                </li>
            {/each}
        </ul>
    </div>
</nav>

<style>
    :global(html) {
		scroll-behavior: smooth;
	}
    nav {
        position: sticky;
        top: 0;
        z-index: 999;
        padding: 0.5em;
        background-color: var(--primary-color);
        color: white;
    }
    img {
        height: 35px;
    }
    .container {
        display: flex;
        align-items: center;
    }
    ul {
        display: flex;
        margin: 0;
        margin-left: auto;
        list-style: none;
        font-size: 1em;
    }
    li {
        margin-right: 20px;
    }
    a {
        text-decoration: none;
        color: #aaa;   
    }
    .active {
        color: white;
    }
</style>