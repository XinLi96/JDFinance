<template>
    <Panel title="神眷满" :class="$style.panel">
        <section :class="$style.content">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t20377/234/1512692244/37538/71f03c74/5b2b878cN1b0824ee.jpg?width=750&height=246" alt="">
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
@import '../../css/element.scss';
.panel{
    @include panel;
    >h4{
        display: none;
    }
    .content{
        img{
            width: 100%;
            height: 230px;
            display: block;
        }
    }
}
</style>
