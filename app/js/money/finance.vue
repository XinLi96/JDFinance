<template>
    <Panel title="理财精选" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t21823/209/1497811121/5076/dfe2d74f/5b2a56b8Nf044e64a.png?width=90&height=90" alt="">
                <div>
                    <h4>月度理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>去赚钱 > </em>
            </div>
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t22465/87/248883325/5159/f8133cd6/5b2a56c7N4c04f536.png?width=90&height=90" alt="">
                <div>
                    <h4>季度理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>去赚钱 > </em>
            </div>
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t22084/101/1500577052/4856/13f8bcb9/5b2a56d9Ne622413c.png?width=90&height=90" alt="">
                <div>
                    <h4>一年理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>
                    <router-link to="index">去赚钱 > </router-link>
                </em>
            </div>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue'
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
    >h4{
        border-bottom: 1px solid #ddd;
    }
    .content{
        @include flex;
        .item{
            @include flex(row);
            align-items: center;
            height: 140px;
            &:after{
                content: ' ';
                box-sizing: border-box;
                height: 0;
                width: 100%;
                border-bottom: 1px solid #ddd;
                margin-left: 140px;
            }
            &:last-child::after{
                border-color: #fff;
            }
            >img{
                width: 88px;
                height: 88px;
                display: inline-block;
                margin: 0 32px;
            }
            >div{
                font-size: 32px;
                color: #333;
                line-height: 1.8;
                width: 344px;
                p{
                    color: #ff3232;
                    font-size: 24px;
                    line-height: 1.1;
                    white-space: nowrap;
                    text-overflow: ellipsis;
                    overflow: hidden;
                }
            }
            >em{
                color: #FF801A;
                font-size: 28px;
            }
        }
    }
}
</style>
