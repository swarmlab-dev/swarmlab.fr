<script>
    import Hero from "./Hero.svelte";
    import What from './What.svelte';
    import TechStack from './TechStack.svelte';
    import Who from './Who.svelte';
    import Partners from './Partners.svelte';
    import Contact from './Contact.svelte';
</script>

<div class="block">
    <div class="child">
        <Hero />
    </div>
    <div class="child">
        <What />
    </div>
    <div class="child">
        <TechStack />
    </div>
    <div class="child">
        <Who />
    </div>
    <div class="child">
        <Partners />
    </div>
    <div class="last">
        <Contact />
    </div>
</div>

<style>
    .child {
        margin-bottom: 5em;
    }
</style>