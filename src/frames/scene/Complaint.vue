<template>
    <section class="child_page">
        <headerTop title="投诉管理"></headerTop>
        <!--info-->
        <div class="listmod">
            <dl>
                <dd>
                    <p class="td">公司<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">上海分公司</span></p>
                </dd>
                <dd>
                    <p class="td">项目<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">回龙观大街</span></p>
                </dd>
                <dd>
                    <p class="td">班组<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">攻壳小组</span></p>
                </dd>
                <dd>
                    <p class="td">被投诉人<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">吴美丽</span></p>
                </dd>
                <dd>
                    <p class="td">日期<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">2017-12-20</span></p>
                </dd>
                <dd>
                    <p class="td">投诉内容<i class="c-chartred">*</i></p>
                    <div class="td tr">
                        <p style="padding-bottom:15px;"><textarea></textarea></p>
                        <p><i class="button">拍照</i><i class="button">从手机相册选择</i></p>
                    </div>
                </dd>
                <dt><i class="button">保存</i><i class="button">提交</i></dt>
            </dl>
        </div>
        <!--info end-->
    </section>
</template>

<script>
  import headerTop from '../../components/Header.vue'
  export default {
    components: {
      headerTop
    },
    data () {
      return {}
    },
    computed: {},
    methods: {}
  }
</script>

<style>
    @import "../../less/site.css";
</style>
