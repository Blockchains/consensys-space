<script>
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
  div {
    max-height: 800px;
    position: relative;
    overflow: auto;
    -webkit-mask-image: linear-gradient(to bottom, black 50%, transparent 100%);
    mask-image: linear-gradient(to bottom, black 50%, transparent 100%);
    z-index: -1;
  }

  .welcome-banner::-webkit-scrollbar {
    display: none;
  }
</style>

<div class="welcome-banner">
  <img {src} alt="c-space image" />
</div>
