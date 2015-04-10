# phalcon框架学习笔记
-------------------

## 视图渲染
- 分层渲染
  ```
    app/views/index.phtml ----> app/views/layouts/controller_name.phtml  ---->  app/views/posts/action_name.phtml
  ```
- 渲染级别

|-类常量 -|	-解释 -|-	顺 序-|
|LEVEL_NO_RENDER |	表明要避免产生任何形式的显示。 |	 |
|LEVEL_ACTION_VIEW |	生成显示到视图关联的动作。| 	1|
|LEVEL_BEFORE_TEMPLATE |	生成显示到控制器模板布局之前。| 	2|
|LEVEL_LAYOUT |	生成显示到控制器布局。| 	3|
|LEVEL_AFTER_TEMPLATE |	生成显示到控制器模板布局后。| 	4|
|LEVEL_MAIN_LAYOUT |	生成显示到主布局。文件： views/index.phtml |	5|
