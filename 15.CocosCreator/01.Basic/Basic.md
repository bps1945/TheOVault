Basic

# 感想

Creator是在抄袭Unity,

但是比较轻量级，比较适合开发轻量级小游戏。

而且对这些微信小游戏，抖音小游戏以及中国本土的这些东西有比较好的支持。

# IDE选择

现在用VSCode作为编辑器因为VSCode对于TypeScript的支持比较好。
CocosDash Board是Electron开发的，因为目录中有.asar 这样的文件
如果这里是2D的状态,要移动画布的话，不是按住中键拖，而是右键。

![](259377aae788072c40235a01e08c54c6.png)


# Gizmo
![](Gizmo.jpg)
①:Move Gizmo
②:Rotate Gizmo
③:Scale Gizmo
④:Rect Gizmo

# GameObject上面绑脚本

![](Basic.3.jpg)

# 点按钮变Label

先在画布上放置一个Button与一个Label

![](Basic.4.jpg)

搞一个controller

![](Basic.5.jpg)

![](Basic.6.jpg)

import { _decorator, Component, Node,Label, Button, director, game, Vec3, Layout, ScrollView, v2} from 'cc';
const { ccclass, property } = _decorator;
@ccclass('TestButtonController')
export class TestButtonController extends Component {
    @property({
        type: Label,
        tooltip: "Add ground prefab owner here",
      })
    public label666: Label = null!;
    public button666: Button = null!;
    start() {
    }
    update(deltaTime: number) {
       
    }
    public testPrintLog() {
        console.log("hello world");  
        this.label666.string="fuckYOU";
    }
}

按钮上的操作

![](Basic.7.jpg)

对齐

![](Basic.1.gif)

# 打图集

图集用TexturePacker就行
![](Basic.2.jpg)

# Prefab的创建

这个就跟unity一样，

从Hierarchy里面把某个节点拖拽到Prefab文件夹里面即可
![](prefab.1.jpg)

# CocosCreator断点调试
![](Basic.8.jpg)

VSCode Chrome插件的安装方法
![](Basic.9.jpg)

安装插件
![](ChromeDebugger.jpg)

然后Add这两个
![](Basic.2.gif)