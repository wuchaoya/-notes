<center>react-native组件</center>


<style>
.platform {
    background-color: #bdebff;
    color: #025268;
    border-radius: 5px;
    margin-right: 5px;
    padding: 0 5px;
    font-size: 13px;
    font-weight: normal;
    -moz-user-select: none;
    -ms-user-select: none;
    -o-user-select: none;
    -webkit-user-select: none;
    user-select: none;

}
</style>
--------------------------
### ActivityIndicator

**属性**

-  `animating`:bool
  是否要显示指示器，默认为true，表示显示。true 不能加""

-  `color`:string
    前景颜色（默认为灰色）

-   <span class="platform">ios</span>`hidesWhenStopped`:bool
    在没有动画的时候，是否要隐藏指示器（默认为true）。

-   `size`: enum('small', 'large')
    指示器的大小。small的高度为20，large为36。
-   `onLayout` :function   
    当组件挂载或者布局发生变化时调用，参数为：
    {nativeEvent: { layout: {x, y, width, height}}}.
  ```html

      <ActivityIndicator
      size="large"
      color="white"
      animating={"false"}
     />
    ```
