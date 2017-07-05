<template>
    <section>
        <headerTop title="统计分析"></headerTop>
        <!--indexmenu-->
        <div class="indexmenu">
            <dl class="layout">
                <dd class="td" @click="toUrl(1)">
                    <i class="ico-per"></i>
                    <p>人员分析</p>
                </dd>
                <dd class="td" @click="toUrl(2)">
                    <i class="ico-item"></i>
                    <p>项目分析</p>
                </dd>
                <dd class="td" @click="toUrl(3)">
                    <i class="ico-user"></i>
                    <p>用工分析</p>
                </dd>
            </dl>
        </div>
        <!--indexmenu end-->
        <!--chart-->
        <div class="chartmod2">
            <h4>出勤人数 | 公司 ∨</h4>
        </div>
        <!--datetab-->
        <div class="datechange">
            <ul class="layout">
                <li class="td">前一天</li>
                <li class="td">出勤 | <em>2017-12-30</em></li>
                <li class="td">后一天</li>
            </ul>
        </div>
        <!--datetab end-->
        <div class="chartmod2">
            <div class="layout">
                <div class="td chartbox"></div>
                <dl class="td chartlist">
                    <dd>
                        <p>20-30岁</p>
                        <p class="c-chartred">47.96%</p>
                    </dd>
                    <dd>
                        <p>30-40岁</p>
                        <p class="c-chartred">47.96%</p>
                    </dd>
                    <dd>
                        <p>40-50岁</p>
                        <p class="c-chartred">47.96%</p>
                    </dd>
                    <dd>
                        <p>50岁以上</p>
                        <p class="c-chartblue">47.96%</p>
                    </dd>
                </dl>
            </div>
        </div>
        <!--chart end-->
        <!--tablue-->
        <table class="an-table">
            <thead>
            <th>序号</th>
            <th>公司名称</th>
            <td>出勤人数</td>
            <th>正常</th>
            <th>异常</th>
            </thead>
            <tbody>
            <tr>
                <td><i>1</i></td>
                <td>北京分公司</td>
                <td>885</td>
                <td>140</td>
                <td>140</td>
            </tr>
            <tr>
                <td><i>2</i></td>
                <td>北京分公司</td>
                <td>885</td>
                <td>140</td>
                <td>140</td>
            </tr>
            <tr>
                <td><i>3</i></td>
                <td>北京分公司</td>
                <td>885</td>
                <td>140</td>
                <td>140</td>
            </tr>
            <tr>
                <td><i>4</i></td>
                <td>北京分公司</td>
                <td>885</td>
                <td>140</td>
                <td>140</td>
            </tr>
            <tr>
                <td><i>5</i></td>
                <td>北京分公司</td>
                <td>885</td>
                <td>140</td>
                <td>140</td>
            </tr>
            </tbody>
        </table>
        <!--tablue end-->
        <footerButtom tab="2"></footerButtom>
        <transition name="router-show">
            <router-view></router-view>
        </transition>
    </section>
</template>

<script>
  import headerTop from '../../components/Header.vue'
  import footerButtom from '../../components/Footer.vue'
  export default {
    components: {
      headerTop,
      footerButtom
    },
    data () {
      return {}
    },
    computed: {},
    methods: {
      toUrl: function (value) {
        let url = ''
        value = parseInt(value) || 0
        switch (value) {
          case 1:
            url = '/stat/staff'
            break
          case 2:
            url = '/stat/project'
            break
          case 3:
            url = '/stat/worker'
            break
        }
        this.$router.push(url)
      }
    }
  }
</script>

<style>
    @import "../../less/analysis.css";
    .router-show-enter-active, .router-show-leave-active {
        transition: all .4s;
    }

    .router-show-enter, .router-show-leave-active {
        transform: translateX(100%)
    }
</style>
