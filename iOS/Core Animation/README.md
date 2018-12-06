# Core Animation

1. Core Animation 是一个复合引擎
    >  Come from Layer Kit

2. CALayer和UIView最大的不同是CALayer不处理用户交互。
   > UIView backing layer, CALayer。
   
   > UIView 提供了处理触摸的具体功能, Core Animation底层方法的高级接口

   > Bridged cast: Use __bridge to convert directly (no change in ownership)

   > 当用代码的方式处理寄宿图，一定设置contentsScale，否则在retina设备显示不正常。
3. CALayer (图层)
   1. contents (寄宿图)
      * contentsGravity
      * contentsScale
      * contentsRect (image sprites)
      * contentsCenter
      > 如果UIView检测到-drawRect: 被调用, 会分配寄宿图，像素尺寸等于 View Size * contentsScale。如果不需要寄宿图，会造成CPU资源和内存浪费。
      
      > CALayerDelegate是一个非正式协议

    |UIView |CALayer |
    |-------|--------|
    |Frame  |Frame   |
    |Bounds |Bounds  |
    |Center |Position|

    frame并不是一个非常清晰的属性，它其实是一个虚拟属性，是根据bounds，position和transform计算而来