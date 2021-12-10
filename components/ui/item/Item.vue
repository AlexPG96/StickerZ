<template>
    <div class="item-card" :style="'box-shadow: ' + boxShadow">
        <div class="item-card-body">
            <div class="item-card-image">
                <a href="#"><fa :icon="icon" /></a>
            </div>
            <div class="item-card-title">
                <p v-html="title" />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: [
        "boxShadow",
        "icon",
        "title"
    ],
}
</script>