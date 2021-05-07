# 目前掌握的选项：

1. el：
   - 类型：string/HTML Element
   - 作用：决定之后Vue实例会管理哪一个DOM。
2. data：
   - 类型：Object/Function（组件当中的data必须是一个函数）
   - 作用：Vue实例对应的数据对象。
3. methods：
   - 类型：{ [key:string] : Function }
   - 作用：定义属于Vue的一些方法。可以在其他地方调用，也可以在指令中调用。