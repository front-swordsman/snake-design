---
imports:
  import TabsDemoCode from '!raw-loader!./simpleTabs.tsx';
  import TabDemo from './simpleTabs.tsx';
  import Code from '../../layout/prism/index'
---

# Tabs 标签页

选项卡切换组件。

### Demo

:::demo
<TabDemo />
:::

## 代码示例

<div><Code>{TabsDemoCode}</Code></div>

## Api

| 属性 | 说明 | 类型 | 默认值 | 必选 |
|:-|:-|:-|:-|:-|
| tabs | tabs 中的展示项 | TabsItemProps[] | [] | 是 |
| activeTab | tab 当前选中页 | number | 0 | 否 |
| onChange | Tab 切换时触发 | Function | | 否 |
| onTabClick | 点击 Tab 时触发 | Function | | 否 |
| tabBarPosition | TabBar位置 | 'top' \| 'bottom \| left \| right | top | 否 |
| tabItemStyle | tabItem 的样式 | React.CSSProperties | | false |
| type | 提供 'line' \| 'card' 两种模式 | string | 'line' | false |
| tabBarUnderlineColor | 下划线颜色 | string | '01C1B2' | false |

## TabsItemProps Api

| 属性 | 说明 | 类型 | 默认值 | 必选 |
|:-|:-|:-|:-|:-|
| title | Tabs 中的单项 | String \| Number \| ReactNode | -- | 是 |
| disabled | Tabs 中的单项是否禁用 | boolean | false | 否 |