<script>
    import Try from '../components/Try.svelte';
import MainPage from '../components/mainPage.svelte';
</script>

<main id="back"class="flex flex-col">
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