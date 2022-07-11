控制应用状态栏的组件
translucent 设置是否透明
 if (VALUE.android) {
    list = list.concat([
      {
        label: '背景色(royalblue)',
        value: 'BackgroundColor',
        type: 'setBackgroundColor',
        params: ['#409EFF', true]
      },
      {
        label: '背景色(default)',
        value: 'BackgroundColor',
        type: 'setBackgroundColor',
        params: ['rgba(0, 0, 0, 0.7)', true]
      },
      {
        label: '透明',
        value: 'Translucent',
        type: 'setTranslucent',
        params: [true]
      },
      {
        label: '不透明',
        value: 'Translucent',
        type: 'setTranslucent',
        params: [false]
      }
    ]);
  }
  return list;