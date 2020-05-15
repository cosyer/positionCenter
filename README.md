# 五种方式实现垂直居中:
- transform
- margin负值
- margin: 0 auto
- display: table
- display: flex

主要代码：
```css
1. transform方式：
.divTransform {
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}
        
2. margin负值方式：
.divMargin {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 300px;
    height: 300px;
    margin-left: -150px;
    margin-top: -150px;
}

3. margin-auto方式
.divMarginAuto {
    position: absolute;
    width: 300px;
    height: 300px;
    margin: auto;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
}

4. display:table方式：
.table {
    display: table;
}

.td {
    display: table-cell;
    vertical-align: middle;
    text-align: center;
}

5. flex方式
.flex {
    display: flex;
    align-items: center;
    justify-content: center;
}
```