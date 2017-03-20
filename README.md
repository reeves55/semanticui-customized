# semanticui-customized

semanticui-customized是方便semantic-ui自定义样式的一个项目，代码是semantic-ui官方代码，按照以下步骤即可自定义semantic-ui的样式

### Semantic UI自定义方法

SemanticUI是一个Web样式库，其中包含了网页开发所用到的常用的控件元素和javascript功能插件，足以满足平常的Web页面开发需要，不同于Bootstrap，SemanticUI提供了很大的自定义空间，自带很多流行的主题，比如Boostrap、Github、Material等，还可以对主题、元素对象样式进行细粒度的自定义。下面简单说说如何自定义SemanticUI的相关主题和元素。

#### 1. 源代码目录结构

![SegmanticUI源代码目录结构](http://blog.reeveslee.com/static/SemanticUI_sourcecode_directory_structure.PNG)

#### 2. 源代码组织架构

![SegmanticUI源代码组织架构](http://blog.reeveslee.com/static/SemanticUI_sourcecode-structure.png)

说明：要想自定义SegmanticUI的主题样式，如果要自定义的属性在 ```definition/elements/***.less```中没有使用变量的值，而是直接定义的，比如说```color: #FEFE08``` ，要修改这些属性的值，就需要直接编辑 ```definiton/elements/***.less```中的属性值；如果要调整的元素的属性值在```definition/elements/***.less```中是一个变量，比如```color:@white```，修改这类属性的值，就需要修改元素所属主题下的```elements/***.variables```文件中对变量值的定义。如果需要更改元素所属主题，直接修改```theme.config```文件中元素的主题属性即可。
