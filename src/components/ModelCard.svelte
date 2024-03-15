<script>
    export let index;
    export let DataFeature

</script>


<div class="grid  gap-14 md:gap-14 lg:gap-20 relative text-base">
    <div class="flex flex-col gap-8 md:gap-10">
        <h4 class="text-2xl sm:text-3xl md:text-4xl max-w-[1000px] w-full font-medium relative pr-10 after:absolute after:top-full after:left-0 after:w-1/5 after:h-1.5 after:mt-1 after:bg-white">
        <slot />
        </h4>
        <p>{DataFeature.description}</p>
        <div class="flex  flex-col gap-3">
            {#each DataFeature.FeatureList as listItem}
                <div class="flex gap-2 item-center">
                    <div class="grip place-item-center px-1.5 text-sm sm:text-sm aspect-square rounded-full border-[1.5px] bg-white border-solid">
                        <i class="fa-solid fa-bolt text-green-400"></i>
                    </div>
                    <p>{listItem}</p>
                </div>
            {/each}
        </div>
    </div>

</div>