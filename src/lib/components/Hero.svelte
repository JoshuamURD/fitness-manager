<script>
  import heroImage from "$assets/Hero.jpg";
  import Button from "$components/Button.svelte";
</script>

<section
  class="relative h-screen bg-cover bg-center bg-no-repeat"
  style="background-image: url('{heroImage}')"
>
  <div
    class="container mx-auto px-4 py-16 text-white from-slate-900/50 via-zinc-900 to-zinc-700 bg-gradient-to-br rounded-lg py-20"
  >
    <h1 class="text-6xl font-bold font-serif mt-4">
      Welcome to fitness manager
    </h1>
    <p class="text-xl font-thin m-2 font-serif">
      Your body as a science experiment. You mad scientist.
    </p>
    <p class="text-lg my-10 mx-2">
      Start pulling in information from various data collection points.
      MyFitnessPal, Hevy and Fitbit come together and then through AI have
      analysis done on your data to help you set better goals for your fitness.
    </p>
    <Button href="/signup">Get started</Button>
  </div>
</section>
