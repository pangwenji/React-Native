按钮组件
 <Button
      onPress={() => {
        this.onPressLearnMore(item);
      }}
      title={item.label}
      color={item.color}
      disabled={item.disabled}
   />
   属性 onPress title color disabled