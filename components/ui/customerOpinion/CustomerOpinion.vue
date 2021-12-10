<template>
    <div class="container py-5">
        <div class="row">
            <div class="col-12 col-md-6">
                <h2 class="title">Free shipping, free online proofs, fast turnaround.</h2>
            </div>
            <div class="col-12 col-md-6 separator">
                <div class="px-3">
                    <div class="customers-icon">
                        <a href="#" class="icon" v-for="(customer, index) in this.customers" :key="index"><fa :icon="customer.image" /></a>
                    </div>
                    <div class="customers-opinion">
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eaque eius, blanditiis quisquam totam, in corrupti impedit animi cupiditate pariatur quam libero, mollitia fugit voluptate error facere autem perferendis sint explicabo.
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

    data() {
        return {
            customers: []
        }
    },

    fetch() {
        this.customers = [
            {
                "title": "All",
                "image": "user-astronaut",
                "opinion": "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eaque eius, blanditiis quisquam totam, in corrupti impedit animi cupiditate pariatur quam libero, mollitia fugit voluptate error facere autem perferendis sint explicabo."
            },
            {
                "title": "All",
                "image": "user-md",
                "opinion": "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eaque eius, blanditiis quisquam totam, in corrupti impedit animi cupiditate pariatur quam libero, mollitia fugit voluptate error facere autem perferendis sint explicabo."
            },
            {
                "title": "All",
                "image": "user-ninja",
                "opinion": "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eaque eius, blanditiis quisquam totam, in corrupti impedit animi cupiditate pariatur quam libero, mollitia fugit voluptate error facere autem perferendis sint explicabo."
            },
            {
                "title": "All",
                "image": "user-tie",
                "opinion": "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eaque eius, blanditiis quisquam totam, in corrupti impedit animi cupiditate pariatur quam libero, mollitia fugit voluptate error facere autem perferendis sint explicabo."
            },
        ];
    }

}
</script>