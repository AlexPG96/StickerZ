<template>
    <div class="container py-5">
        <div class="row">
            <div class="col-12 col-md-6">
                <img class="sticker-image" src="../../../assets/img/stiker.png" alt="StikerZ">
            </div>
            <div class="col-12 col-md-6 d-flex flex-wrap align-self-center">
                <div class="grid-text" v-for="(step, index) in this.steps" :key="index">
                    <ItemText 
                    :stepNumber="step.stepNumber"
                    :stepColor="step.stepColor"
                    :stepTitle="step.stepTitle"
                    :stepDescription="step.stepDescription" />

                </div>
            </div>
        </div>
    </div>
  
</template>

<script>
export default {
    
    data() {
        return {
            steps: [],
        }
    },

    fetch() {
        this.steps = [
            {
                "stepNumber": "01",
                "stepColor": "#9757D7",
                "stepTitle": "Step 1",
                "stepDescription": "Track your workouts, get beeter results, and be the best version of you."
            },
            {
                "stepNumber": "02",
                "stepColor": "#EF466F",
                "stepTitle": "Step 2",
                "stepDescription": "Wheter you're a complete beginner or you want to step up your routine."
            },
            {
                "stepNumber": "03",
                "stepColor": "#45B26B",
                "stepTitle": "Step 3",
                "stepDescription": "Print custom stickers in any shape or size on premium vinyl don't stress."
            },
            {
                "stepNumber": "04",
                "stepColor": "#FFB62A",
                "stepTitle": "Step 4",
                "stepDescription": "Get the full studio experience at home with thousands of classes for body, mind."
            },
        ]
    }

}
</script>