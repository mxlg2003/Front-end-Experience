#### 重写element-ui组件样式

注：在带scoped的style标签里面重写element-ui组件样式失效，可以使用 >>> 或 /deep/ 来解决
原因是scoped是当前组件的唯一标识，针对第三方组件（element-ui）的样式无效

1. css 可以使用 >>> 或 /deep/ （#form 是父级元素）
```css
<style scoped>
#form /deep/ .el-button{
    background: red;
}
// 或
#form >>> .el-button{
    background: red;
}
</style>
```
2. less 只能使用 /deep/  （#form 是父级元素）
```css
<style lang="less" scoped>
#form {
   /deep/ .el-button{
        background: red;
    }
}
 
</style>
```
