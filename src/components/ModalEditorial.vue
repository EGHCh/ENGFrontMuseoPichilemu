<template>
  <div class="container-fluid editorial-modal mt-sm-5 fixed-bottom d-flex">
    <div class="modal-container py-4 px-2">
      <h3 class="modal-title">EDITORIAL</h3>
      <hr />
      <p class="px-4 mt-2 px-sm-4">
        A museum (from Latin, musēum and this, in turn, from the Greek,
        Μουσείον) is a public or private institution, permanent, for profit or
        non-profit, at the service of society and its development, and open to
        the public, which acquires, preserves, researches, communicates,
        exhibits, for study and educational purposes, collections of art,
        scientific, among others, always with cultural value, according to the
        International Council of Museums (ICOM).2 The science that studies them
        is called museology, the technique of their management museography and
        their administration, museonomy.
        <br />
        <br />
        Museums exhibit collections, that is, sets of objects and information
        that reflect some aspect of human existence or its environment. These
        types of collections, almost always valuable, have existed since ancient
        times: objects of worship or offerings were kept in temples that from
        time to time were exhibited to the public so that they could contemplate
        and admire them. The same thing happened with the valuable objects and
        works of art collected by some people of the aristocracy in Greece and
        Rome; they had them exposed in their homes, in their gardens and proudly
        taught them to friends and visitors. It was in the Renaissance when the
        name of "museum" was given as it is understood today to buildings
        expressly dedicated to the conservation and exhibition of their
        permanent collections. On the other hand, there are art galleries, where
        paintings and sculptures are shown, in temporary exhibitions, without
        necessarily having permanent collections. Its name derives from the
        galleries (of palaces and castles), which were the spacious lobbies with
        an elongated shape, with many windows or open and supported by columns
        or pillars, intended for moments of rest and the exhibition of
        ornamental objects, often works of art.
        <br />
        <br />
        After World War I (1918), the International Museum Office emerged, which
        articulated the museographic criteria whose programs and technical
        solutions are in force today. In 1945 the International Council of
        Museums (ICOM) was born and in 1948 the periodical Museum appears
        through which the activities of museums around the world are
        disseminated to this day. (Source: Paragraphs of the description of
        Wikipedia..).
      </p>
      <button class="modal-close" @click="closeModal">
        <img src="../assets/close.png" alt="" />
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ModalEditorial",
  methods: {
    closeModal: function () {
      document.querySelector(".editorial-modal").classList.add("d-none");
      document.querySelector(".editorial-modal").classList.remove("d-flex");
    },
  },
};
</script>

<style>
.editorial-modal {
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
.editorial-modal .modal-container {
  height: 70vh;
  max-width: 700px;
  background-image: url(https://images.unsplash.com/photo-1615800098779-1be32e60cca3?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2020&q=80);
  background-attachment: fixed;
}
.editorial-modal .modal-container .modal-title {
  font-size: 24px;
  font-weight: bold;
  line-height: 24px;
}
.editorial-modal .modal-container p {
  max-height: 70%;
  overflow: scroll;
}
.editorial-modal .modal-close {
  border: none;
  background: rgba(0, 0, 0, 0);
  margin-top: 1rem;
}
</style>
