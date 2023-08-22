<script>
    import logo from "$lib/assets/logo-dark-line.png";
    const year = new Date().getFullYear();
</script>

<footer>
    <div class="container">
        <img src={logo} alt="SwarmLab"/>
        <span>- {year} - All Rights Reserved.</span>
    </div>
</footer>

<style>
    img {
        height: 25px;
        vertical-align:middle;
    }
    span {
        vertical-align:middle;
    }
    footer {
        padding: 3em 0;
        background-color: var(--primary-color);
        color: white;
    }
    .container {
        text-align: center;
    }
</style>