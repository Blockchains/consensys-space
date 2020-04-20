<script>
  import { onMount } from "svelte";

  var imageSet = [
    "https://consensys-space-assets.s3.amazonaws.com/cover01.jpg",
    "https://consensys-space-assets.s3.amazonaws.com/cover02.jpg",
    "https://consensys-space-assets.s3.amazonaws.com/cover03.jpg",
    "https://consensys-space-assets.s3.amazonaws.com/cover04.jpg",
    "https://consensys-space-assets.s3.amazonaws.com/cover05.jpg"
  ];

  let index = 0;
  let src = imageSet[0];

  setInterval(() => {
    index++;
    if (index === imageSet.length) {
      index = 0;
    }
    src = imageSet[index];
  }, 1000);
</script>

<style>

</style>

<div>
  <img {src} alt="c-space image" />
</div>
