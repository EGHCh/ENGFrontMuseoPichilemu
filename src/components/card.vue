<template>
  <div class="">
    <div class="card">
      <img :src="picture_src" class="card-img-top" :alt="cardTitle" />
      <div class="card-body">
        <h5 class="card-title">{{ cardTitle }}</h5>
        <div class="card-text-container">

          <p class="card-text">
            {{ cardBody }}
        </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardTemplate",
  components: {},
  props: {
    picture_src: String,
    cardTitle: String,
    cardBody: String,
  },
};
</script>

<style>
.card {
  max-width: 260px;
  height: 360px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  cursor: pointer;
  margin-bottom: 1rem;
  overflow: hidden;
}
.card .card-img-top {
  height: 50%;
  object-fit: cover;
  object-position: 0% 15%;
}
.card .card-body {
  font-family: "Roboto Mono", monospace;
  max-height: 55%;
  background-color: rgba(233, 138, 21, 0.5);
}
.card .card-title {
  font-size: 20px;
  line-height: 27px;
  font-weight: bold;
}
.card .card-text-container {
  height: 60px;
  overflow: hidden;
}
.card .card-text {
  font-size: 14px;
  line-height: 15px;
  height: 100px;
  display: -webkit-box;
  overflow: hidden;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
}
@media (min-width: 400px) {
  .card {
    width: 18rem;
  }
}
</style>
