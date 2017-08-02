## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/stjava/getapi/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/stjava/getapi/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
1. IDEA简介 
摘自百度百科：IDEA 全称IntelliJ IDEA，是java语言开发的集成环境，IntelliJ在业界被公认为最好的java开发工具之一，尤其在智能代码助手、代码自动提示、重构、J2EE支持、Ant、JUnit、CVS整合、代码审查、 创新的GUI设计等方面的功能可以说是超常的。
个人体会：用了IDEA几天，个人感觉IDEA的开发体验还是很不错的，但是上手难度可能比Eclipse高，需要一定的学习成本。
2.IDEA的安装
	可以从官网下载安装，速度还是蛮快的。https://www.jetbrains.com/idea/。
具体安装步骤并没有特别需要注意的地方，直接下一步即可。
3.开始使用
打开IDEA后，跳过初始化设置，进入如下界面。
 
左侧可以选择最近打开的项目，右侧可以快速新建、导入、打开项目。此时我们选择新建一个项目（Create New Project）
4.新建一个spring-boot项目
第一步：设置项目JDK
在左侧选择Spring Initializr，然后右侧选择jdk，如果没有，需要下载jdk然后安装，安装完成，点击New，选择安装目录导入。项目服务器初始化目录选择Default即可。然后点击Next。
 
第二步：设置项目信息
Group：	maven的组名称，一般为com.公司名称
Artifact：项目名称
Type：选择Maven
其余如下
 
第三步：选择项目依赖包
	左侧选择类型，中间选择具体的包，右侧是已经选择的，这个项目只是一个简单的spring demo 项目，所以只用选择下web包即可。后期可以根据具体的需求导入相关的Maven依赖配置，如mysql jdbc redis mongoDB等，这里这是一个通过选择来配置pom.xml的简化配置。
 
第四步：设置项目名称和路径
 
5.搭建一个SPRING-WEB DEMO访问
上一步设置完成，就进入了项目开发界面，类似Eclipse，左侧为项目文件目录，右侧为代码开发区。
 
在左侧找到DemoApplication
 
增加@RestController注解，此注解会让当前类的所有方法默认都以JSON形式返回
同时新增返回hello world 方法，然后右键Run

 
当控制台打印输出如下时，就证明项目正常启动，此时打开浏览器，输入localhost:8080，即可查看结果。
 
 


