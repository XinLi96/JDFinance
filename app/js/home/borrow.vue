<template>
    <Panel title="极速借贷" :class="$style.panel">
        <section :class="content">
            <router-link :to="{ name : 'home' }">
                <img src="//img30.360buyimg.com/jr_image/jfs/t19387/129/150574595/59759/b2eca8ad/5a601a54N70f4d416.png" alt="">
            </router-link>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
export default {
    components: {
        Panel,
    }
}
</script>

<style lang="scss" module>
@import "../../css/element.scss";
.panel{
    @include panel;
    .content{
        padding-bottom: 40px;
        img{
            display: block;
            width: 100%;
        }
    }
}
</style>
