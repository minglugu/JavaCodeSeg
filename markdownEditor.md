# 页面.html
<div id="editor"> </div>

# 初始化.js
// 初始化编辑器
var editor = editormd("editor", {
    // 尺寸必须在这里设置，设置样式会被 editormd 自动覆盖掉
    width: "100%",
    // 设定编辑器高度
    height: "500px",
    // 编辑器中的初始化内容
    markdown: "# 在这里写下一篇博客",
    // 指定 editor.md 依赖的插件路径
    path: "editor.md/lib/"
});

# 获得编辑框的内容.js
// 获取 markdown 格式的数据
editor.getMarkdown();
// 获取 html 格式的数据
editor.getHTML();

# 引入依赖.html
<!-- 引入 editor.md 的 dependency 
    注意：引入的文件路径，和项目中保存的路径一致-->
<link rel="stylesheet" href="editor.md/css/editormd.min.css" />
<script src="js/jquery.min.js"></script>
<script src="editor.md/lib/marked.min.js"></script>
<script src="editor.md/lib/prettify.min.js"></script>
<script src="editor.md/editormd.js"></script>