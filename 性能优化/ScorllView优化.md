 一、 
  如果要优化首次加载速度，也就是启动速度：可以参考 TAT.ronnie 的文章中的方法，根据实际情况，最小化 ScrollView 或者 ListView 初始子项数量；
优化内存：因为 ScrollView/ListView 会保存所有子 View 在内存中，因为我们没法删掉子项，但是我们可以尽量减少每个子项所占的内存。例如这个项目 react-native-sglistview，它在子项不可见的时候，就把它退化成一个最基本的 View
二、https://www.race604.com/react-native-scrollview-performance/