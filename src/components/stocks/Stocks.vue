<template>
    <div>
        <app-stock v-for="stock in stocks" :key="stock.id" :stock="stock"></app-stock>
    </div>
</template>

<script>
import Stock from './Stock';

export default {
    data() {
        return {
            stocks: [
                { id: 1, name: 'BMW', price: 200 },
                { id: 2, name: 'Google', price: 140 },
                { id: 3, name: 'Apple', price: 220 },
                { id: 4, name: 'Twitter', price: 120 },
            ]
        }
    },
    components: {
        appStock: Stock
    }
}
</script>