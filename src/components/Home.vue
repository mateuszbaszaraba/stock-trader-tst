<template>
    <div>
        <h1>Trade or view your portfolio</h1>
        <h6>You can save & load</h6>
        <hr>
        <p>Your Funds: {{ funds | currency }}</p>
    </div>
</template>

<script>
export default {
    computed: {
        funds() {
            return this.$store.getters.funds
        }
    }
}
</script>