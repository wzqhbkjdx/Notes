**这是测试文档2**

_下次会添加一些干货了_

**ok干货来啦**

android View 的事件体系 读《Android开发艺术探索》by 任玉刚

> 什么是View

*   View是android中所有控件的基类。
*   View的属性

      Left

      Right

      Top

      Bottom

      x

      y

      translationX

      translationY

_View在平移的过程中，top和left表示的是原始左上角的位置信息，其值并不会发生改变，此时发生改变的是x y translationX translationY。_

*   MotionEvient

      ACTION_DOWN

      ACTION_UP

      ACTION_MOVE

      getX

      getY

      getRawX

      getRawY

*   TouchSlop

      系统所能识别出的被认为是滑动的最小距离

      ViewConfiguration.get(getContext()).getScaledTouchSlop()

*   组织结构划分

*   开发流程

*   UML