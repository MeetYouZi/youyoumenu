# youyoumenu 使用说明

## 安装

```

yarn install youyoumenu

```

### 引入

```

import youyoumenu from 'youyoumenu'

```

### 使用

```vue

<youyoumenu
  v-for="item in list"
  :menu="item"
  :key="item.index"
  @openMenu="openMenu"
  :openedMenus="openedMenus"
>
</youyoumenu>

```

### 使用数据结构

```vue

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
            title: '主菜单',
            list: [
              {
                index: '1-1',
                name: '子菜单'
              },
            ]
          }
        ]
      }]
    }
  }
}
</script>

```

