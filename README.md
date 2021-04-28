## 2.15.3【2021年4月25日】
el-table对于expandRow增加class=“el-table__expanded-row”方便做动画

## 2.15.2【2021年4月16日】
修复el-tooltip、el-popover，使用匿名函数创建on事件但是使用具名函数off，导致eventlistener不销毁的内存溢出的问题

## 2.15.1
修复el-table表格开启了翻页勾选的功能后，创建的store不销毁导致的内存溢出的问题