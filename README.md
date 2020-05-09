# 快速使用rem移动端自适应
## 安装
```
npm install imrem
```
## 使用
### main.js文件中引入;
```
import 'imrem';
```
### 安装外部插件px转换rem
> #### 安装
>  > 打开Visual Studio Code，扩展，在应用商店中搜索：cssrem ; 安装好重启Visual Studio Code;
> 
>  > 左上角文件 -> 首选项 -> 设置 -> 搜索中输入cssrem；
> #### cssrem设置
> * "cssrem.autoRemovePrefixZero": true
>  > 默认打勾
> * "cssrem.fixedDigits": 6 
>  > px转rem小数点最大长度，默认：6。
> * "cssrem.ingoresViaCommand": []
>  > 自动移除0开头的前缀，默认：true
> * "cssrem.rootFontSize": 75
>  > (重点就是这个了) 这里就是设置基础的font-size，如果设计图是750标准的（iphone6），则设置成75。设计图为375，则设置成37.5；
>  > (设计图尺寸多大就填多大!!! )
##### 说明
```
页面中使用，设计图上面多少尺寸，直接填多大，自动转换为rem。
例如：设计图上面某个按钮尺寸宽80px，代码中直接：width:80px;会自动弹出rem转换，选择转换的rem单位即可。
```
#### 即下即用！