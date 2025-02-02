![image](http://wx1.sinaimg.cn/large/a73bc6a1ly1fz9rutoazqj21kw0lon0r.jpg)  

>ArtQRCode 是基于 qrcode.js 的封装，支持以图片元素为基本单元的二维码绘制。

## Basic Usages
```js
<div id="qrcode"></div>
<script>
    var options = {
        text: "https://github.com/252860883/ArtQRCode",
        width: 500,
        height: 500,
        codeWidth: 320,
        codeHeight: 320,
        top: 85,
        left: 80,
        /**
         * materials unit options
         */
        materials: {
            border: "./materials/electron/border.png",
            eye: "./materials/electron/eye.png",
            row4: "./materials/electron/row4.png",
            col4: "./materials/electron/col3.png",
            row2col3: "./materials/electron/row2col3.png",
            row3col2: "./materials/electron/row3col2.png",
            col3: ["./materials/electron/col3.png", "./materials/electron/col3_2.png"],
            row2col2: "./materials/electron/row2col2.png",
            corner: "./materials/electron/corner.png",
            row2: ["./materials/electron/row2.png", "./materials/electron/row2_2.png"],
            col2: "./materials/electron/col2.png",
            single: ["./materials/electron/single.png", "./materials/electron/single_2.png"],
        }
    }
   /**
    * when the artqrcode loaded, run this function
    */
    function callBack(status) {
        console.log(status) // [loaded|success]
    }
    var qrcode = new QRCode(document.getElementById("qrcode"), options, callBack);
</script>
```

## Material Configuration
想要生产出好看的二维码，图片素材必不可少。这需要设计师按照固定比例进行设计，具体素材命名以及规范如下：

![image](https://wx1.sinaimg.cn/large/a73bc6a1ly1g7pse7pdf7j22dx0l3ae2.jpg)

![image](https://wx2.sinaimg.cn/large/a73bc6a1ly1g7pr17yjbgg21mn0m5jx5.gif)

## Productive Example
![image](http://wx2.sinaimg.cn/large/a73bc6a1ly1fmeydtz4jej21kw0qzgz6.jpg)


## Last
- 觉得有意思的话，给颗star吧～
- 网罗一线牵，珍惜这段缘
- We meet in the network,please cherish this fate
- 欢迎issue
