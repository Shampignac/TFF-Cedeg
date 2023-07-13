<template>
  <div
    class="flex flex-col items-center justify-center h-screen bg-black text-white"
  >
    <h1 class="text-6xl font-bold mb-4">Oups! Erreur 404</h1>
    <p class="text-xl mt-8">
      C'est un peu gênant... On dirait que cette page s'est perdue dans
      l'espace.
    </p>
    <div class="gif-container">
      <img
        src="public\medias\IMG_4147.gif"
        alt="GIF Error 404"
        class="w-80 h-auto"
      />
    </div>
  </div>
</template>

<style>
.gif-container {
  margin-top: 2rem;
}

@media (min-width: 768px) {
  .gif-container {
    max-width: 400px;
  }
}
</style>
