csspretty.vim  
@Author 闲耘™<hotoo.cn[AT]gmail.com>  
@Modifier lilydjwg <lilydjwg@gmail.com>  

csspretty for vim.

这个脚本基于[http://www.vim.org/scripts/script.php?script_id=2137](CSS Pretty:
Pretty-print a css file)修改而来。

原基准脚本中使用 split 方法分割 ":" 来区分 css 属性和值，并且值(value)只取分割
出来的第二项，当值本身带有冒号（如 URL）时，就会截断忽略后面的部分。

目前已经修正了这个问题，并补充了一些其他的特性，比如自动根据`&sw`使用用户的缩进
设置。如果希望左大括号在新行中，vimrc 中设置`let g:CssPrettyLeftBraceAtNewLine=1`即可。

如果左大括号不在新行，其前会添加一个空格。
