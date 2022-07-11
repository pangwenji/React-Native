 ScrollView（滚动视图）的组件，同时还集成了触摸锁定的“响应者”系统。

记住 ScrollView 必须有一个确定的高度才能正常工作，因为它实际上所做的就是将一系列不确定高度的子组件装进一个确定高度的容器（通过滚动操作）。要给 ScrollView 一个确定的高度的话，要么直接给它设置高度（不建议），要么确定所有的父容器都有确定的高度。一般来说我们会给 ScrollView 设置flex: 1以使其自动填充父容器的空余空间，但前提条件是所有的父容器本身也设置了 flex 或者指定了高度，否则就会导致无法正常滚动，你可以使用元素查看器来查找具体哪一层高度不正确。

 {
    label: '横向/竖向滚动',
    value: 'horizontalScroll',
    type: 'horizontalScroll'
  },
  {
    label: '禁止滚动',
    value: 'scrollEnabled',
    type: 'scrollEnabled'
  },
  {
    label: '显示水平滚动条',
    value: 'showsHorizontalScrollIndicator',
    type: 'showsHorizontalScrollIndicator'
  },
  {
    label: '显示垂直滚动条',
    value: 'showsVerticalScrollIndicator',
    type: 'showsVerticalScrollIndicator'
  },
  {
    label: '末尾禁止弹性拉动',
    value: 'bounces',
    type: 'bounces'
  },
  {
    label: '去顶部',
    value: 'scrollTo'
  },
  {
    label: '去底部',
    value: 'scrollToEnd'
  },
  {
    label: '启用下拉刷新',
    value: 'refreshControl',
    type: 'RefreshControl'
  }