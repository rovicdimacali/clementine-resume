<template>
  <div
    class="pdf-container"
    style="
      display: flex;
      flex-direction: column;
      align-items: stretch;
      width: 100%;
      text-align: center;
      gap: 20px;
    "
  >
    <a
      href="https://res.cloudinary.com/dpm5vdakr/image/upload/v1714916388/Clementine_Villongco_Resume_ghzf7o.pdf"
      >Download Resume</a
    >
    <VuePdfEmbed
      source="https://res.cloudinary.com/dpm5vdakr/image/upload/v1714916388/Clementine_Villongco_Resume_ghzf7o.pdf"
      style="max-width: 1200px; width: 100%; margin: 0 auto"
    />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.vue-pdf-embed__page {
  max-width: 1200px;
  margin: 0 auto;
}

a {
  text-decoration: none;
  padding: 10px 15px;
  background: orange;
  color: white;
  font-family: sans-serif;
  font-weight: 700;
  margin: 20px auto;
  border-radius: 15px;
  animation: myAnim 2s ease 0s infinite normal forwards;
}

@keyframes myAnim {
  0%,
  100% {
    transform: rotate(0deg);
    transform-origin: 50% 50%;
  }

  10% {
    transform: rotate(4deg);
  }

  20%,
  40%,
  60% {
    transform: rotate(-5deg);
  }

  30%,
  50%,
  70% {
    transform: rotate(5deg);
  }

  80% {
    transform: rotate(-4deg);
  }

  90% {
    transform: rotate(4deg);
  }
}
</style>
