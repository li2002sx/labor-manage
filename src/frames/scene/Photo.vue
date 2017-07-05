<template>
    <section class="child_page">
        <headerTop title="工人照片录入"></headerTop>
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
                    <p class="td">工人<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">张三丰</span></p>
                </dd>
                <dd>
                    <p class="td">照片类型<i class="c-chartred">*</i></p>
                    <p class="td tr"><span class="after">操作证</span></p>
                </dd>
                <dd>
                    <p class="td">照片<i class="c-chartred">*</i></p>
                    <p class="td tr"><i class="button">拍照</i><i class="button">从手机相册选择</i></p>
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
