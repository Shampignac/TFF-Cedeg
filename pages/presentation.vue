<template>
  <div class="min-h-screen">
    <main class="pt-10 pb-40 px-5 relative">
      <div
        class="absolute top-0 left-0 right-0 bottom-0 z-0"
        style="
          background-image: url('../public/medias/Green-Life.png');
          background-size: cover;
          background-position: center;
          opacity: 0.4;
        "
      ></div>
      <section class="mb-10">
        <h2 class="text-3xl font-semibold mb-4 text-yellow-400">
          Qui sommes-nous ?
        </h2>
        <p class="text-lg text-sky-700">
          Chez GreenLife, nous sommes passionnés par l'écologie et la
          préservation de l'environnement. Notre entreprise vise à promouvoir un
          mode de vie durable et respectueux de la planète.
        </p>
      </section>

      <section class="mb-10">
        <h2 class="text-3xl font-semibold mb-4 text-yellow-400">
          Notre Mission
        </h2>
        <p class="text-lg text-sky-700">
          Notre mission est de sensibiliser les individus et les entreprises aux
          défis environnementaux actuels et de leur offrir des solutions
          écologiques pour contribuer à la protection de la nature et de la
          biodiversité.
        </p>
      </section>

      <section class="mb-10">
        <h2 class="text-3xl font-semibold mb-4 text-yellow-400">
          Nos Services
        </h2>
        <ul class="list-disc list-inside text-lg text-sky-700">
          <li>Conseils en développement durable</li>
          <li>Solutions énergétiques renouvelables</li>
          <li>Gestion des déchets</li>
          <li>Produits écologiques</li>
        </ul>
      </section>
    </main>
    <div class="top-0 bottom-0 left-0 right-0 bg-emerald-200 p-5">
      <h2 class="text-2xl font-semibold mb-4">Contact</h2>
      <form class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div>
          <label for="name" class="block text-gray-700 font-medium mb-2"
            >Nom :</label
          >
          <input
            type="text"
            id="name"
            class="w-full rounded-lg border px-4 py-2 focus:outline-none focus:ring focus:border-blue-300"
            placeholder="Votre nom"
          />
        </div>
        <div>
          <label for="prénom" class="block text-gray-700 font-medium mb-2"
            >Prénom :</label
          >
          <input
            type="text"
            id="prénom"
            class="w-full rounded-lg border px-4 py-2 focus:outline-none focus:ring focus:border-blue-300"
            placeholder="Votre prénom"
          />
        </div>
        <div>
          <label for="email" class="block text-gray-700 font-medium mb-2"
            >Email :</label
          >
          <input
            type="email"
            id="email"
            class="w-full rounded-lg border px-4 py-2 focus:outline-none focus:ring focus:border-blue-300"
            placeholder="Votre email"
          />
        </div>
        <div>
          <label for="message" class="block text-gray-700 font-medium mb-2"
            >Message :</label
          >
          <textarea
            id="message"
            class="w-full rounded-lg border px-4 py-2 focus:outline-none focus:ring focus:border-blue-300"
            placeholder="Votre message"
          ></textarea>
        </div>
        <div class="col-span-2">
          <button
            type="submit"
            class="bg-blue-500 text-white font-semibold px-4 py-2 rounded-lg hover:bg-blue-600 transition-colors duration-300"
          >
            Envoyer
          </button>
        </div>
      </form>
    </div>
    <div class="bg-green-500 py-4 text-white text-center">
      <p class="text-lg">
        Contactez-nous :
        <a
          href="mailto:contact@greenlife.com?subject=Je%20suis%20intéressé%20par%20GreenLife"
          class="text-white"
          >contact@greenlife.com</a
        >
      </p>
    </div>
  </div>
</template>


<style>
.custom-text {
  color: #fdfdfd;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 2); /* Ombre portée pour améliorer la lisibilité */
}

@media (min-width: 768px) {
  .grid-cols-1 {
    grid-template-columns: 1fr;
  }

  .md:grid-cols-2 {
    grid-template-columns: 1fr 1fr;
  }

  .md:order-1 {
    order: 1;
  }

  .md:order-2 {
    order: 2;
  }
}

@media (max-width: 640px) {
  .mb-10 {
    margin-bottom: 2rem;
  }

  .grid-cols-1 {
    grid-template-columns: 1fr;
  }

  .md\:grid-cols-2 {
    grid-template-columns: 1fr;
  }

  .col-span-2 {
    grid-column: 1 / -1;
  }

  .bg-emerald-200 {
    padding: 1rem;
  }
}
</style>
