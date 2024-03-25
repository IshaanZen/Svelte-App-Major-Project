<script>
  import ModelCard from "./ModelCard.svelte";
import SectionWrapper from "./section-wrapper.svelte";


let DataFeature= [
    {
        FeatureList: [
            '12000+ Audio Data Samples Used','6 Set of Different Emotions' , 'Both CNN and RNN Models Used' , 'Higher Accuracy Than Before'
        ] ,
        description:"Voice Sense Our cutting-edge emotion recognition AI employs sophisticated algorithms to meticulously analyze vocal  as asda effortlessly discerning a spectrum of emotional states. ",
         imgUrl: 'assets/Models.png'
    } ,
 
    {
        FeatureList: [
            'RAVDESS Emotional speech audio','Crowd Sourced Emotional Multimodal Actors Dataset (CREMA-D)' , 'Toronto emotional speech set (TESS) ' , 'Surrey Audio-Visual Expressed Emotion (Savee)'
        ] ,
        description:"Dataset is a collection of various types of data stored in a digital format. Data is the key component of any Machine Learning project." ,
        imgUrl: 'assets/Datasets.png'
    } 
  ] 

</script>

<SectionWrapper class="">
  <div
    class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:pb-14"
  >
    <div class="flex flex-col gap-2">
      <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
        Realise what <span class="text-indigo-400">FEELING</span> is in your mind
      </p>
      <h3
        class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
      >
        Feature Extraction Model
      </h3>
    </div>

    {#each DataFeature as DataFeature, index}
      <ModelCard {DataFeature} {index}>
        {#if index === 0}
            Surveillance 
        {:else if index === 1}
            Dataset Used
        <!-- {:else} -->
        {/if}
      </ModelCard>
    {/each}
  </div>
</SectionWrapper>
