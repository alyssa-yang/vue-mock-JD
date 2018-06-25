<template>
   <Panel title="公司信息" :class="$style.panel">
       <ul :class="$style.content">
           <li>
               <router-link :to="{name:'home'}">
                   <img src="//img12.360buyimg.com/jrpmobile/jfs/t17587/158/1300523690/1908/eabacaac/5ac4850bNdf876dd8.png?width=60&height=60"/>
                   <p>首页</p>
               </router-link >
           </li>
           <li>
               <router-link :to="{name:'home'}">
                   <img src="//img12.360buyimg.com/jrpmobile/jfs/t7690/252/3621724688/1715/757a3ca1/59e9d81bN27304850.png?width=60&height=60"/>
                   <p>理财</p>
               </router-link >
           </li>
           <li>
               <router-link :to="{name:'home'}">
                   <img src="//img12.360buyimg.com/jrpmobile/jfs/t11653/76/201131398/1192/bf1b2852/59e9d7f3N5f691137.png?width=60&height=60"/>
                   <p>白条</p>
               </router-link >
           </li>
           <li>
               <router-link :to="{name:'home'}">
                   <img src="//img12.360buyimg.com/jrpmobile/jfs/t19729/201/1027312338/1395/95cecd48/5ab85d0eN01f81011.png?width=56&height=56"/>
                   <p>省钱</p>
               </router-link >
           </li>
            <li>
               <router-link :to="{name:'home'}">
                   <img src="//img12.360buyimg.com/jrpmobile/jfs/t10897/141/1894216742/2046/ad0e8dc1/59e9d7feNaa5dd2fd.png?width=60&height=60"/>
                   <p>金融会员</p>
               </router-link >
           </li>
       </ul>
   </Panel>
   
</template>

<script>
import Panel from "../core/panel.vue"
export default {
    components: {
        Panel,
    },
}
</script>
<style lang="scss" module >
@import "../../css/element.scss";
.panel {
  @include panel;
  position: fixed;
  left: 0;
  right: 0px;
  bottom: 0px;
  height: 100px;
  margin: 0px;
  z-index: 2;
  > h4 {
    display: none;
  }
  .content {
    @include flex(row);
    justify-content: space-around;
    padding: 10px 0;
    li {
      text-align: center;
      a {
        text-decoration: none;
      }
      img {
        width: 44px;
        height: 44px;
        display: inline-block;
      }
      p {
        font-size: 22px;
        color: #656565;
      }
    }
  }
}
</style>
