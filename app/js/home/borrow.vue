

<template lang="html">
    <Panel title="极速借贷" :class="$style.panel">
        <section :class="$style.content">
            <router-link :to="{name:'home'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t21127/208/43135801/40227/1d6a4e4/5af6ec1eNe8ca1622.jpg?width=750&height=320"/>
            </router-link>
        </section>
    </Panel>
</template>


<script>
import Panel from "../core/panel"

export default {
    components: {
        Panel,
    },
}
</script>


<style lang="scss" module>
@import "../../css/element.scss";
.panel {
  @include panel;
  .content {
    padding-bottom: 40px;
    img {
      display: block;
      width: 100%;
    }
  }
}
</style>
