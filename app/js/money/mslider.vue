<template>
    <Panel title="轮播图" :class="$style.panel">
        <section :class="$style.content">
            <Slider :items="items" :cname="$style.slider"></Slider>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
import Slider from '../core/slider.vue';
export default {
    components: {
        Panel,
        Slider,
    },
    data(){
        return{
            items: [{
                href: 'home',
                src: '//img12.360buyimg.com/jrpmobile/jfs/t20725/51/1733032054/24475/fb4205ce/5b3379c0N8e86a8ac.jpg?width=750&height=400'
            },{
                href: 'home',
                src: '//img12.360buyimg.com/jrpmobile/jfs/t20935/229/1706320157/40828/33874fe6/5b3379dcN0dd211f6.jpg?width=750&height=400',
            }]
        }
    }
}
</script>

<style lang="scss" module>
@import "../../css/element.scss";
.panel{
    @include panel;
    >h4{
        display: none;
    }
    .content{
        .slider{
            margin-top: 120px;
        }
    }
}
</style>
