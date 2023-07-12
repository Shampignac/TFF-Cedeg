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
      <span class="md:ml-2 text-white text-xl font-bold mt-4 md:mt-0">{{
        siteName
      }}</span>
    </div>
    <nav class="container mt-4">
      <ul class="flex flex-wrap md:flex-nowrap">
        <li class="relative mr-4">
          <nuxt-link to="/" class="text-white hover:text-primary-light">{{
            menuItems.home
          }}</nuxt-link>
        </li>
        <li class="relative mr-4">
          <nuxt-link
            to="/presentation"
            class="text-white hover:text-primary-light"
            >{{ menuItems.greenLife }}</nuxt-link
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
                >{{ menuItems.presentation }}</nuxt-link
              >
            </li>
            <li>
              <nuxt-link
                to="/produits"
                class="text-white hover:text-primary-light"
                >{{ menuItems.produits }}</nuxt-link
              >
            </li>
            <li>
              <nuxt-link
                to="/conseils"
                class="text-white hover:text-primary-light"
                >{{ menuItems.conseils }}</nuxt-link
              >
            </li>
          </ul>
        </li>
        <li class="relative mr-4">
          <nuxt-link
            to="/formation"
            class="text-white hover:text-primary-light"
            >{{ menuItems.formation }}</nuxt-link
          >
        </li>
        <li class="relative mr-4">
          <nuxt-link to="/stage" class="text-white hover:text-primary-light">{{
            menuItems.stage
          }}</nuxt-link>
        </li>
        <li>
          <nuxt-link
            to="/developpement-professionnel"
            class="text-white hover:text-primary-light"
            >{{ menuItems.developpementProfessionnel }}</nuxt-link
          >
        </li>
      </ul>
    </nav>
    <div class="container mt-8 text-white text-center">
      <p>Tous droits réservés &copy; {{ currentYear }} {{ companyName }}</p>
      <div class="mt-4">
        <nuxt-link to="/charte" class="text-white hover:text-primary-light">{{
          menuItems.charte
        }}</nuxt-link>
        <span class="mx-2 text-white">|</span>
        <nuxt-link
          to="/politique-confidentialite"
          class="text-white hover:text-primary-light"
          >{{ menuItems.politiqueConfidentialite }}</nuxt-link
        >
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      showSubMenu: false,
      siteName:
        "TFF de Jérôme Marchand dans le cadre de la formation de Web-Dev",
      companyName: "Shampignac",
      currentYear: new Date().getFullYear(),
      menuItems: {
        home: "Accueil",
        greenLife: "GreenLife",
        presentation: "Présentation",
        produits: "Produits",
        conseils: "Conseils",
        formation: "Formation",
        stage: "Stage",
        developpementProfessionnel: "Développement Professionnel",
        charte: "Charte",
        politiqueConfidentialite: "Politique de Confidentialité",
      },
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
