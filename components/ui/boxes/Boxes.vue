<template>
    <div class="container py-5">
        <div class="row">
            <div class="col-12 col-md-3 text-center" v-for="(item, index) in this.arrItems" :key="index">
                <Item
                    :boxShadow="item.boxShadow"
                    :icon="item.icon" 
                    :title="item.title" />
            </div>
        </div>
    </div>
</template>

<script>
export default {

    data() {
        return {
            arrItems: [],
        }
    },

    fetch() {
        this.arrItems = [
            {
                "boxShadow": "0 0 0 1.25rem rgba(236, 236, 252, 1)",
                "icon": "tags",
                "title": "Labels"
            },
            {
                "boxShadow": "0 0 0 1.25rem rgba(245, 233, 221, 1)",
                "icon": "shopping-bag",
                "title": "Bags"
            },
            {
                "boxShadow": "0 0 0 1.25rem rgba(241, 220, 238, 1)",
                "icon": "boxes",
                "title": "Boxes"
            },
            {
                "boxShadow": "0 0 0 1.25rem rgba(233, 234, 214, 1)",
                "icon": "tape",
                "title": "Tape"
            },
        ]
    }

}
</script>

<style>

</style>