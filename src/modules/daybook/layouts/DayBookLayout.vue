<template>
    <Navbar />

    <div class="d-flex ">
        <div class="col-4 bg-success">
            <EntryList />
        </div>
        <div class="col bg-secondary">
            <router-view />
        </div>
    </div>
</template>

<script>
import {defineAsyncComponent} from 'vue'

export default {
    components: {
        Navbar: defineAsyncComponent(() => import('../components/Navbar')),
        EntryList: defineAsyncComponent(() => import('../components/EntryList')),
    },
}
</script>