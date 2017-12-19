这是我自己的笔记。by tanzx

记录一些问题：
1 低版本的refresh方法，默认pageNumber是1，但是高版本的refresh方法需要指定pageNumber。使用高版本时，如果不写pageNumber，那么pageNumber就是当前页。
在数据变少时调用refresh方法就会查不到数据。
2 缺少一个remove方法。表格的一行的最后一列有一个删除按钮时，点击删除按钮删除当前行不方便。点击删除按钮时，可以获取4个参数(e, value, row, index)。
使用row参数可以写出一个删除行的好方法。页面中就可以调用这个好方法来实现删除功能。然而在bootstrap-table中没有实现这个好方法。
