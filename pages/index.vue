<template>
  <div>
    <main class="relative">
      <div
        class="absolute top-0 left-0 right-0 bottom-0 z-0"
        style="
          background-image: url('/medias/hackerman.jpg');
          background-size: cover;
          background-position: center;
          opacity: 0.6;
        "
      ></div>
      <div class="container mx-auto px-6 py-12 relative z-10">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <div class="md:order-2">
            <h1 class="text-4xl font-bold mb-4 custom-text">
              Beaucoup de choses me passionnent.
            </h1>
            <p class="text-lg mb-4 custom-text">
              Peut-être parfois un petit peu trop. Je suis quelqu’un
              d’autodidacte, toujours à l’affût de nouvelles compétences, mais
              cela me porte préjudice parfois, car je passe d’une compétence à
              une autre rapidement.
            </p>
            <p class="text-lg custom-text">
              Cependant, en prenant de l’âge, je me suis rendu compte que toutes
              ces compétences se sont rejointes et font sens dans des liens que
              j’arrive à utiliser dans de nombreux projets de ma vie.
            </p>
          </div>
          <div class="md:order-1">
            <h1 class="text-4xl font-bold mb-4 custom-text">
              L’outil informatique occupe une place prépondérante dans ma vie.
            </h1>
            <p class="text-lg mb-4 custom-text">
              Dès l'âge de 12 ans, je démontais et remontais la tour de mon
              ordinateur, récupérant des pièces ici et là pour augmenter ses
              capacités. Cela m'a donné des compétences en hardware dès mon plus
              jeune âge.
            </p>
            <p class="text-lg mb-4 custom-text">
              Ensuite, j'ai passé beaucoup de temps à chercher des logiciels et
              jeux, poussant toujours plus loin les limites de mon ordinateur.
              Cela m'a permis de développer la capacité de m’adapter très
              rapidement à tout nouveau logiciel rencontré.
            </p>
            <p class="text-lg custom-text">
              A tel point que j’ai acquis cette capacité à faire des liens entre
              toutes mes connaissances et à maîtriser de nouveaux logiciels en
              quelques heures. Je n’ai pas la prétention de dire que j’ai un don
              dans ce domaine, mais cette somme d’expériences a construit
              quelque chose d’unique qui me permet de comprendre et de
              m’approprier rapidement tout nouveau concept.
            </p>
          </div>
        </div>
        <div class="mt-8">
          <h1 class="text-4xl font-bold mb-4 custom-text">
            Lors du début de ma formation en mars, j'étais au niveau 0 en
            développement web.
          </h1>
          <p class="text-lg mb-4 custom-text">
            C'est grâce à l'enseignement de Julien Broens que j'ai réussi, comme
            j'aime si bien le dire, à « écarter la brume » qui entoure le
            développement web pour les profanes.
          </p>
          <p class="text-lg custom-text">
            Je suis conscient qu'il me reste encore beaucoup à apprendre, mais
            désormais, je dispose des outils que j'associe à mes autres
            compétences, ce qui me permet d'avoir l'opportunité de proposer et
            de créer des choses nouvelles et propres à mon univers.
          </p>
        </div>
      </div>
    </main>
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
</style>
