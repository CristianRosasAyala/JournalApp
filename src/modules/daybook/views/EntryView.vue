<template>
    <div class="entry-title d-flex justify-content-between p-2">
        <div>
            <span class=" text-success fs-3 fw-bold">15</span>
            <span class=" mx-1 fs-3">Julio</span>
            <span class=" mx-2 fs-4 fw-light">2021, jueves</span>
        </div>

        <div>
            <button class=" btn btn-danger mx-2">
                Borrar
                <i class="fa fa-trash-alt"></i>
            </button>
            <button class=" btn btn-primary mx-2">
                Subir foto
                <i class="fa fa-upload"></i>
            </button>
        </div>
    </div>

    <div class=" d-flex flex-column px-3 h-75">
        <textarea class=" bg-secondary" placeholder="¿Qué sucedió hoy?"></textarea>
    </div>

    <Fab icon="fa-save"/>

    <img class=" img-thumbnail" src="https://cdn.hobbyconsolas.com/sites/navi.axelspringer.es/public/styles/950/public/media/image/2021/05/chainsaw-man-2322987.jpg?itok=k6_QGiLZ" alt="entry picture">
    <hr>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        Fab: defineAsyncComponent(()=> import('../components/Fba.vue')),
    },
}
</script>

<style lang="scss" scoped>

    textarea{
        font-size: 20px;
        border: none;
        height: 100%;

        &:focus {
            outline: none;
        }
    }

    img{
        width: 200px;
        position: fixed;
        bottom: 150px;
        right: 20px;
        box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 1.0);
    }

</style>