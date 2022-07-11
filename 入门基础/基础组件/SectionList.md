列表组件
完全跨平台。
行组件显示或隐藏时可配置回调事件。
支持单独的头部组件。
支持单独的尾部组件。
支持自定义行间分隔线。
支持分组的头部组件。
支持分组的分隔线。
支持多种数据源结构
支持下拉刷新。
支持上拉加载。
 <SectionList
          renderItem={({ item, index, section }) => (
            <Text
              key={index}
              style={{
                borderBottomWidth: 1,
                borderBottomColor: '#eee',
                textAlign: 'center',
                height: 40,
                lineHeight: 40
              }}
            >
              {item}
            </Text>
          )}
          renderSectionHeader={({ section: { title } }) => (
            <Text
              style={{
                fontWeight: 'bold',
                padding: 4,
                fontSize: 16,
                backgroundColor: '#eee'
              }}
            >
              {title}
            </Text>
          )}
          sections={SECTIONS}
          keyExtractor={(item, index) => item + index}