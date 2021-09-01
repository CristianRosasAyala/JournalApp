<template>
  <div @click="$router.push({name: 'entry', params: { id:10}})" class="entry-container pointer p-3">
      <div class="entry-title d-flex">
          <span class=" text-primary fs-5 fw-bold">15</span>
          <span class="mx-1 fs-5">Julio</span>
          <span class="mx-2 fw-light">2021, Jueves</span>
      </div>

      <div class="entry-description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium odio, voluptate quas atque maiores rem est ipsam soluta maxime earum velit, aspernatur natus minima magni dolor eaque sunt facere hic laudantium delectus. Omnis, velit illum? Sit dolores rerum commodi nesciunt.
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.entry-container{
    border-bottom: 1px solid #2c3e50;
    
    transition: 0.1s all ease-in;

    &:hover {
        background-color: lighten($color: grey, $amount: 15);
        transition: 0.1s all ease-in;
    }
}

.entry-description{
    font-size: 12px;
}
</style>