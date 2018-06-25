<template lang="html">
    <div>
       <HomeHeader/>
       <HomeSilder/>
       <Novice/>
       <Borrow/>
       <Money/>
       <Product/>
       <Life/>
       <HomeFooter/>
       <Navbar/>
    </div>
</template>

<script>
import HomeHeader from "../public/header.vue"
import HomeFooter from "../public/footer.vue"
import Navbar from "../public/navbar.vue"
import HomeSilder from "./homeSilder.vue"
import Novice from "./novice.vue"
import Borrow from "./borrow.vue"
import Money from "./money.vue"
import Product from "./product.vue"
import Life from "./life.vue"

export default {
    components: {
        HomeHeader,
        HomeFooter,
        HomeSilder,
        Novice,
        Borrow,
        Money,
        Product,
        Life,
        Navbar,
    },
}
</script>

