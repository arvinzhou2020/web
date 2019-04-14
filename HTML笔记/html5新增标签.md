\# html5+css3  是之前的一个升级
### html5
    1.语义化标签 
    2.新增表单属性以元素
    3.存储  
    4.地理定位  
    5.文件上传及读取
    6.音频视频
    canvas！！扩展
### css3：
    过渡
    动画
    2d    旋转   放大   移动  扭曲
    3d    旋转   放大   移动  扭曲（立体效果）
    flex：
### 移动web：（移动端布局）
    百分比布局   %

    flex：布局；

    rem布局：

    响应式布局（框架）： bootstrap；

## 1.语义化标签：  
    1.针对于移动端  
    2.ie9不支持（会把语义化标签当做行内元素）----转换为display:block  
    3.ie6 7（不认识语义化标签） ---js创建元素在转化为块元素。
        1.header头部标签
        2.nav：导航标签
        3.main：主体标签
        4.article：文章
        5.aside：侧边栏
        6.footer：底部标签
        7.section：某一个区域部分
## 2.音频：
    audio   
        1.src:音频的来源
        2.controls:控制器  
        3.autoplay：自动播放 
        4.loop:循环播放
## 3.视频：
    video: 
        1.autoplay:自动播放 
        2.controls：控制器 
        3.width与height只设置一个等比例放大缩小
        4.loop：循环  
        5.src路径  
        6.poster：当浏览器打开的时候默认显示的第一帧（画面）
        7.muted：静音播放。（js可以控制解决）
## 4.input新增标签元素   (要有form 表单  submit提交)
    1.url：网址（合法的网址）
    2.email：邮箱
    3.date：日期
    4.time：当前时间
    5.week：周
    6.number：数字键盘  只能输入数字
    7.tel：数字键盘  只能输入数字
    8.search：人性化体验
    9.表单分组：
            <fieldset align="center">
                 当前组的标题
                <legend>hello</legend>
            </fieldset>
    10.  下拉列表   要与input与datalist结合使用   input里面list的属性值与datalist里面的id值保持一致（绑定）
        <input type="text" list="a">
        <datalist id="a">
            <option value="张三" label="hello"></option>
            <option value="李四"></option>
            <option value="王五"></option>
        </datalist>
## 5.表单属性：
    1.required： 必须输入的
    2.placeholder:默认提示符（占位符）
    3.autofocus:默认获取焦点
    4.autocomplete：提示符  off|on  1.必须有name属性 2.必须提交过 3.在form表单里面
    5.multiple:可以选择多个文件  
    6.disabled 禁止用户操作。
## 6.css3之属性选择器：
    1.div[class]  标签名[属性]   --- 选择div且包含属性为class
    2.[class]  [属性]  只要是包含class属性
    3. div[class=boxa]  标签名[属性=属性值]。
    4. div[class^=box]  以box类名开头的。
    5.div[class$=b]  以b结尾的。
    6.div[class*=o]  包含o就会被选中。
## 7.结构选择器：
    1.:first-child
    2.last-child
    3.nth-child(n)
    4.nth-of-type(n)
## 8.伪元素选择器：
    ::before在当前元素的前面   ::after在当前元素的后面     content：""    行内元素
    ::first-letter  首字母
    ::first-line  首行
    ::selection  选中样式的修饰
## 9.css3 之 2d：
###1.移动：
      写法：
         1.transform:translate(水平,垂直)   2.transform:translateX(水平)  3.2.transform:translateY(垂直)  
        注意： 1.根据自身移动  2.对行内元素无效 
###2.旋转
       1.transform:rotate(30deg)   2.rotateY()   3.rotateX()
        1.旋转默认中心点旋转   正值是顺时针   负值是逆时针
###3.缩放
        transform:scale(2)  数值 
            两个值  第一个值代表水平放大或缩小  第一个值代表垂直放大或缩小   
#### 4.倾斜（扭曲）
        1.transform: skew(ndeg);  2.transform: skewX(ndeg)  3.transform: skewY(ndeg)
    可以写多个：
        transform: translate() rotate() scale() skew();
        旋转可以旋转坐标轴！！！
## 10. 动画
    animation: 动画名字  动画时间  运动曲线  动画何时开始  播放次数  是否反方向   结束的状态；
    任何动画  做完之后都会回到原来的位置（状态）！！