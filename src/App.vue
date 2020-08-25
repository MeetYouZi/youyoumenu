<template>
  <div id="app">
    <youyoumenu
      v-for="item in list"
      :menu="item"
      :key="item.index"
      :openedMenus="openedMenus"
    ></youyoumenu>
  </div>
</template>

<script>
export default {
  data () {
    return {
      list: [
        {
          index: '1',
          title: '产品',
          collapse: false,
          children: [
            {
              index: '1-0',
              title: '惟数平台',
              list: [
                {
                  index: '1-1',
                  name: '惟数平台综述'
                }, {
                  index: '1-2',
                  name: '实时开发平台'
                }, {
                  index: '1-3',
                  name: '离线开发平台'
                }, {
                  index: '1-4',
                  name: '数据资产管理平台'
                }, {
                  index: '1-5',
                  name: '机器学习平台'
                }
              ]
            }, {
              title: '惟客宝',
              list: [
                {
                  index: '1-3',
                  name: '电商云'
                }, {
                  index: '1-4',
                  name: '营销云'
                }, {
                  index: '1-5',
                  name: '导购云'
                }, {
                  index: '1-6',
                  name: '客户云'
                }, {
                  index: '1-7',
                  name: '客流云'
                }, {
                  index: '1-8',
                  name: '分析云'
                }
              ]
            }, {
              title: '运营服务',
              list: [
                {
                  index: '1-9',
                  name: '营销代教服务'
                }
              ]
            }
          ]
        }, {
          index: '2',
          title: '解决方案',
          collapse: false,
          children: [
            {
              index: '2-0',
              subTitle: '商业地产'
            }, {
              index: '2-1',
              subTitle: '医药零售'
            }, {
              index: '2-2',
              subTitle: '教育培训'
            }, {
              index: '2-3',
              subTitle: '鞋服家居'
            }
          ]
        }, {
          index: '3',
          title: '客户案例',
          collapse: false,
          children: [
            {
              index: '3-0',
              title: '惟数平台',
              list: [
                {
                  index: '3-1',
                  name: '惟数平台综述'
                }, {
                  index: '3-2',
                  name: '实时开发平台'
                }
              ]
            }, {
              index: '3-3',
              title: '惟客宝',
              list: [
                {
                  index: '3-4',
                  name: '惟数平台综述1'
                }, {
                  index: '3-5',
                  name: '实时开发平台1'
                }
              ]
            }
          ]
        }, {
          index: '4',
          title: '惟客动态',
          collapse: false,
          children: [
            {
              index: '4-0',
              subTitle: '新闻事件'
            }, {
              index: '4-1',
              subTitle: '活动报道'
            }, {
              index: '4-2',
              subTitle: '行业专题'
            }
          ]
        }, {
          index: '5',
          title: '关于我们',
          collapse: false,
          children: [
            {
              index: '5-0',
              title: '公司介绍'
            }, {
              index: '5-1',
              title: '核心团队'
            }, {
              index: '5-2',
              title: '荣誉资质'
            }, {
              index: '5-3',
              title: '加入我们'
            }
          ]
        }
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
