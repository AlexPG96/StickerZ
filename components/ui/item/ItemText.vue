<template>
    <div class="text-block">
        <div class="step-block" v-html="stepNumber" :style="'background-color: ' + stepColor"/>
        <div class="step-title" v-html="stepTitle" />
        <div class="step-text" v-html="stepDescription" />
    </div>
</template>

<script>
export default {

    props: [
        "stepNumber",
        "stepColor",
        "stepTitle",
        "stepDescription"
    ]

}
</script>