## 2.15.7【2021年5月7日】
el-cascader级联选择器开发的时候加了console，忘记移除了，现在去掉

## 2.15.6【2021年5月6日】
el-cascader级联选择器开启了filterable可搜索之后，二次点击无法收回下拉框的问题

## 2.15.5【2021年5月6日】
el-table方法cell-dblclick方法修改为取event.target.innerText，取字段原生的值因为经常格式化，导致复制的不正确

## 2.15.4【2021年5月6日】
el-table方法cell-dblclick方法新增复制功能，使用原生复制execCommand进行复制，不进行引用vue-clipboard2插件，调用顺序为:

双击事件-》进行复制-》抛出cell-dblclick事件

## 2.15.3【2021年4月25日】
el-table对于expandRow增加class=“el-table__expanded-row”方便做动画

## 2.15.2【2021年4月16日】
修复el-tooltip、el-popover，使用匿名函数创建on事件但是使用具名函数off，导致eventlistener不销毁的内存溢出的问题

## 2.15.1
修复el-table表格开启了翻页勾选的功能后，创建的store不销毁导致的内存溢出的问题