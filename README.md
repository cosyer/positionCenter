#三种方式实现垂直居中:transform:translate方式,margin方式以及display:table方式

主要代码：

    1、transform方式：
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
            
    2、margin方式：
    .divMargin {
                position: absolute;
                top: 50%;
                left: 50%;
                width: 300px;
                height: 200px;
                margin-left: -150px;
                margin-top: -100px;
            }
    
    3、display:table方式：
    .table {
                display: table;
            }
    
            .td {
                display: table-cell;
                vertical-align: middle;
                text-align: center;
            }