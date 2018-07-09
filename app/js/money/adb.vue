<template>
    <Panel title="理财专享" :class="$style.panel">
        <section :class="$style.content">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t21520/220/770346544/34912/890a3c18/5b17a40fNb6732372.jpg?width=750&height=200" alt="">
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
            height: 170px;
            display: block;
        }
    }
}
</style>
