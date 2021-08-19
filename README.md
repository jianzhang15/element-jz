## 2.16.8【2021年8月19日】
增加el-tooltip可以换行展示

## 2.16.7【2021年8月17日】
移除el-collapse空格会导致收起的问题

## 2.16.5【2021年8月7日】
修改el-message默认的topOffset从20改为10
修改el-dialog打开关闭动画，动画效果更强

## 2.16.4【2021年8月6日】
表格没有列，会只有1列的情况下不展示，展示的时候fadeIn，体验更好

## 2.16.2【2021年7月27日】
修复el-checkbox参与min设置的情况下is-disabled和is-checked并存的样式冲突问题

## 2.16.1【2021年7月22日】
解决el-checkbox多选的情况下样式错乱由于is-focus导致的问题

## 2.15.9【2021年6月7日】
解决el-menu submen路由重复maxstack的问题

## 2.15.8【2021年5月8日】
解决el-table双击复制的时候如果里面是el-switch空的内容，也会提示复制成功

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