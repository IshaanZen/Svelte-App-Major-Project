<script>
    import Try from '../components/Try.svelte';
    import MainPage from '../components/mainPage.svelte';
    import { onMount } from 'svelte';

    onMount(()=>{
        let scroll = new LocomotiveScroll({
      el: document.querySelector('[data-scroll-container]'),
      smooth: true
    });
    })
</script>
<link rel="stylesheet" href="../src/Stylesheets/locomotive.css">
<main id="back"class="flex flex-col" data-scroll-container>
    <MainPage/>
    <Try/>

</main>

<style>
    #back{
    background: linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.7)) , url("/src/images/back-g.jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100vw;
    height: 100vh;
    }


</style>