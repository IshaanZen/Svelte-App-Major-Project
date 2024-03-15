<script>
    import Try from "./Try.svelte"
    import Header from "./header.svelte";
import SectionWrapper from "./section-wrapper.svelte";
</script>

<SectionWrapper>

    <Header/>
    <div class="flex flex-col gap-10 flex-1 items-center justify-center pb-10 md:pb-14 flex-wrap">
        <h2 class=" uppercase text-5xl sm:text-6xl md:text-7xl lg:text-8xl max-w-[1400px] mx-auto w-full">
            Emotion <span class=" border-2 rounded-3xl p-2 px-2">Detection</span> Sysytem
        </h2>
        
        <button id="try-btn" >
            Try Now !!! 
            
            <span></span><span></span><span></span><span></span>
            <i class="fa-solid fa-arrow-up-right-from-square"></i>
        </button>
        
    <p class="mx-10 p-6">~ Stress or worry is like a rocking chair , It gives you something to do but never gets you anywhere</p>
    </div>

    <!-- <Try/> -->

    

</SectionWrapper>

<style>

</style>