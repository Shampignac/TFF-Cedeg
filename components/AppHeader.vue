<template>
  <header class="bg-primary-dark py-4 pb-24">
    <div
      class="container flex flex-col md:flex-row items-center justify-between"
    >
      <nuxt-link to="/">
        <div class="rounded-full bg-white p-1">
          <img
            src="/medias/Logo-Centre-Cedeg.png"
            alt="Logo"
            class="h-20 w-20 rounded-full w-auto"
          />
        </div>
      </nuxt-link>
      <span class="md:ml-2 text-white text-xl font-bold mt-4 md:mt-0"
        >TFF de Jérôme Marchand dans le cadre de la formation de Web-Dev</span
      >
    </div>
    <nav class="container  mt-4">
      <ul class="flex flex-wrap  md:flex-nowrap">
        <li class="relative mr-4">
          <nuxt-link to="/" class="text-white hover:text-primary-light"
            >Accueil</nuxt-link
          >
        </li>
        <li class="relative mr-4">
          <nuxt-link
            to="/presentation"
            class="text-white hover:text-primary-light"
            @mouseenter="showSubMenu = true"
            @mouseleave="hideSubMenu"
            >GreenLife</nuxt-link
          >
          <ul
            class="absolute bg-primary-dark mt-2 py-2 px-4 rounded-lg"
            v-show="showSubMenu"
            @mouseenter="showSubMenu = true"
            @mouseleave="hideSubMenu"
          >
            <li>
              <nuxt-link
                to="/presentation"
                class="text-white hover:text-primary-light"
                >Présentation</nuxt-link
              >
            </li>
            <li>
              <nuxt-link
                to="/produits"
                class="text-white hover:text-primary-light"
                >Produits</nuxt-link
              >
            </li>
            <li>
              <nuxt-link
                to="/conseils"
                class="text-white hover:text-primary-light"
                >Conseils</nuxt-link
              >
            </li>
          </ul>
        </li>
        <li class="relative mr-4">
          <nuxt-link to="/formation" class="text-white hover:text-primary-light"
            >Formation</nuxt-link
          >
        </li>
        <li class="relative mr-4">
          <nuxt-link to="/stage" class="text-white hover:text-primary-light"
            >Stage</nuxt-link
          >
        </li>
        <li>
          <nuxt-link
            to="/developpement-professionnel"
            class="text-white hover:text-primary-light"
            >Développement Professionnel</nuxt-link
          >
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      showSubMenu: false,
    };
  },
  methods: {
    hideSubMenu() {
      setTimeout(() => {
        this.showSubMenu = false;
      }, 5000);
    },
  },
};
</script>

<style>
.container {
  max-width: 1140px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 1rem;
  padding-right: 1rem;
}

.bg-primary-dark {
  background-color: #0e0b09;
}

.bg-primary {
  background-color: #151e28;
}

@media (min-width: 768px) {
  .flex-nowrap {
    flex-wrap: nowrap;
  }

  .md:flex-row {
    flex-direction: row;
  }

  .md:ml-2 {
    margin-left: 0.5rem;
  }

  .md:mt-0 {
    margin-top: 0;
  }
}
</style>
