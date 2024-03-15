<script>
  import ModelCard from "./ModelCard.svelte";
import SectionWrapper from "./section-wrapper.svelte";


let DataFeature= [
    {
        FeatureList: [
            '1500+ Audio Data Samples Used','6 Set of Different Emotions' , 'Both CNN and RNN Models Used' , 'Higher Accuracy Than Before'
        ] ,
        description:"Voice Sense Our cutting-edge emotion recognition AI employs sophisticated algorithms to meticulously analyze vocal  as asda effortlessly discerning a spectrum of emotional states. This application excels in delivering a comprehensive emotional analysis offering valuable insights into individual emotions and overall sentiment. By harnessing advanced technology, our platform elevates the understanding of emotional nuances providing users with a nuanced and insightful perspective on the emotional landscape. As pioneers in the field of emotion recognition we are dedicated to offering a refined and insightful experience that goes beyond conventional boundaries",
        imgUrl: ''
    } 
] 
//     {
//         FeatureList: [
//             '1500+ Audio Data Samples Used','6 Set of Different Emotions' , 'Both CNN and RNN Models Used' , 'Higher Accuracy Than Before'
//         ] ,
//         description:"Voice Sense Our cutting-edge emotion recognition AI employs sophisticated algorithms to meticulously analyze vocal  as asda effortlessly discerning a spectrum of emotional states. This application excels in delivering a comprehensive emotional analysis offering valuable insights into individual emotions and overall sentiment. By harnessing advanced technology, our platform elevates the understanding of emotional nuances providing users with a nuanced and insightful perspective on the emotional landscape. As pioneers in the field of emotion recognition we are dedicated to offering a refined and insightful experience that goes beyond conventional boundaries",
//         imgUrl: ''
//     } , 
//     {
//         FeatureList: [
//             '1500+ Audio Data Samples Used','6 Set of Different Emotions' , 'Both CNN and RNN Models Used' , 'Higher Accuracy Than Before'
//         ] ,
//         description:"Voice Sense Our cutting-edge emotion recognition AI employs sophisticated algorithms to meticulously analyze vocal  as asda effortlessly discerning a spectrum of emotional states. This application excels in delivering a comprehensive emotional analysis offering valuable insights into individual emotions and overall sentiment. By harnessing advanced technology, our platform elevates the understanding of emotional nuances providing users with a nuanced and insightful perspective on the emotional landscape. As pioneers in the field of emotion recognition we are dedicated to offering a refined and insightful experience that goes beyond conventional boundaries",
//         imgUrl: ''
//     }



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
        <!-- {:else if index === 1}
        {:else} -->
        {/if}
      </ModelCard>
    {/each}
  </div>
</SectionWrapper>
