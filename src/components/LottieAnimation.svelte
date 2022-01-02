<script>
  import { LottiePlayer } from "@lottiefiles/svelte-lottie-player";
  let fetchJson = fetch("lotties/coder-lottie.json").then((res) => res.json());
</script>

{#await fetchJson}
  <p>...</p>
{:then result}
  <LottiePlayer
    src="/lotties/coder-lottie.json"
    autoplay={true}
    loop={true}
    renderer="svg"
    background="transparent"
    height={400}
    width={400}
  />
{/await}
