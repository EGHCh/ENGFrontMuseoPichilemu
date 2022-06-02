<template>
  <div class="container-fluid patrimonio-modal mt-sm-5 fixed-bottom d-flex">
    <div class="modal-container py-4 px-2">
      <h3 class="modal-title mt-2">What do we understand by cultural heritage?</h3>
      <hr />
      <p class="pb-4 px-sm-4">
        <strong>Cultural heritage</strong> is a certain set of tangible,
        intangible and natural assets that are part of social practices, to
        which values are attributed to be transmitted, and then resignified,
        from one era to the next, or from one generation to the next. Thus, an
        object is transformed into a heritage or cultural asset, or ceases to
        be, through a process and/or when someone - individual or collectivity -
        affirms its new condition (Dibam, Memory, culture and creation.
        Political guidelines. Document, Santiago, 2005).
        <br />
        <br />
        he fact that cultural heritage is conformed from a social and cultural
        process of attribution of values, functions and meanings, implies that
        it is not something given once and for all but, rather, it is the
        product of a permanent, complex and controversial social process, with
        mixed feelings and meanings. Thus, the protected objects and assets
        acquire reason for being to the extent that they open up to new meanings
        and are associated with a present culture that contextualizes, recreates
        and interprets them in a dynamic way.
        <br />
        <br />
        The value of these cultural goods and manifestations is not in a
        faithfully rescued past, but in the relationship that people and
        societies establish in the present, with such traces and testimonies.
        Therefore, citizens are not mere passive recipients but subjects who
        know and transform that reality, making possible the emergence of new
        interpretations and patrimonial uses. As UNESCO has stressed, the term
        "cultural heritage" has not always had the same meaning, and in recent
        decades it has undergone a profound change. Today, this is a more open
        notion that also includes expressions of the present culture, and not
        only of the past.
        <br />
        <br />
        On the other hand, if at one point this concept was referred exclusively
        to monuments, it has now gradually incorporated new categories such as
        those of intangible, ethnographic or industrial heritage, which, in
        turn, have required new conceptualization efforts. Along with this,
        greater attention has been given to the arts of representation,
        languages and traditional music, as well as to the philosophical,
        spiritual and information systems that constitute the framework of these
        creations.

        <br />
        Source: National Cultural Heritage Service
      </p>
      <button class="modal-close" @click="closeModal">
        <img src="../assets/close.png" alt="" />
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ModalPatrimonio",
  methods: {
    closeModal: function () {
      document.querySelector(".patrimonio-modal").classList.add("d-none");
      document.querySelector(".patrimonio-modal").classList.remove("d-flex");
    },
  },
};
</script>

<style>
.patrimonio-modal {
  box-sizing: border-box;
  top: 0;
  width: 100vw;
  height: 100vh;
  z-index: 1999;
  background-color: rgba(0, 0, 0, 0.5);
  align-items: center;
  justify-content: center;
  font-family: "Old Standard TT", serif;
}
.patrimonio-modal .modal-container {
  height: 70vh;
  max-width: 700px;
  background-image: url(https://images.unsplash.com/photo-1615800098779-1be32e60cca3?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2020&q=80);
  background-attachment: fixed;
}
.modal-container .modal-title {
  font-size: 24px;
  font-weight: bold;
  line-height: 24px;
}
.modal-container p {
  max-height: 70%;
  overflow: scroll;
}
.modal-close {
  border: none;
  background: rgba(0, 0, 0, 0);
  margin-top: 1rem;
}
</style>
