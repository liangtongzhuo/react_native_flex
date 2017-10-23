# react-native flex 布局

![](1.png)

react-native 就下面四种 flex 属性控制布局。
```
const styles = StyleSheet.create({
  container: {
    backgroundColor: '#fff',
  },
  item: {
    backgroundColor: '#4385f5',
    color: 'white',
    textAlign: 'center',
    fontSize: 50,
    lineHeight: 100,
    width: 100,
    height: 100,
    margin: 5,
  },
  //flexDirection（主轴）
  //column（默认 从上向下）| column-reverse |  row | row-reverse 
  box_flexDirection: {
    flexDirection: 'column'
  },
  //justifyContent（描述子盒子之间的距离）
  //flex-start（默认 从右边开始）| flex-end | center | space-between（两端靠边，项目之间间距相等）| space-around（每个项目两侧的间隔相等）
  //需要 item 宽高调整小一些，才可以看见效果
  box_justifyContent: {
    justifyContent: 'flex-start',
    flexDirection: 'row',    
  },
  //flexWrap （描述一行排满是否换行） 
  //nowrap（默认 不换行）| wrap 
  box_flexWrap: {
    flexWrap: 'wrap',
    flexDirection: 'row',
  },
  //alignItems（用于描述交叉轴（又名 侧轴））
  //flex-start（默认）| flex-end | center | baseline（第一行字体对齐）| stretch（侧轴方向撑满）
  box_alignItems: {
    alignItems: 'flex-start'
  },
});
  ```
