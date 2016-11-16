# PDFViewAndDownload
iOS开发 PDF文件的浏览与加载

## 简要说明
在实际的开发过程中，我们会遇到一些需要显示PDF的场景，比如一些表单，比如官方文件（为了保证原有的格式显示正常，通常会做成PDF来展示），这里我们来讨论一个展示PDF的方式。
包括本地加载与网络加载，另外附带了PDF文件的几种下载方式，供大家参考。
* UIWebView 这是一种通用的方式，对于本地的PDF展示也是如此，只要把上面的fileName换成本地的文件地址即可。但是这个方式有个很大的弊端，就是只有最基本的展示，不能放大缩小，也没有其他的相关交互，当然，混编除外，可是有必要这样做吗？对于已经处理好的PDF而且仅仅最基本展示，这种方式最方便。
* 利用CGContextDrawPDFPage，这种方式我并不熟悉，所以这里只是提一下，有兴趣的朋友可以自己找一下相关资料。
* QLPreviewController 这是系统提供的预览方式，其实展示起来效果也差不多，支持放大缩小的手势，还自带系统分享功能。  
* 使用强大的第三方[Reader(vfr)](https://github.com/vfr/Reader)，这个很强大，功能很多，也提供了一些自定义的控制常量。诸如`READER_FLAT_UI`的。想要扩展的话，可以自己改写ReadViewController文件

具体内容请参见源码

有任何问题可以一起讨论，联系我：hllfj922@gmail.com

