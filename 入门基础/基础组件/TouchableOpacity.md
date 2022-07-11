本组件用于封装视图，使其可以正确响应触摸操作。当按下的时候，封装的视图的不透明度会降低
<TouchableOpacity
        style={styles.button}
        onPress={onPress}
      >
        <Text>Press Here</Text>
      </TouchableOpacity>