# 第一章 介绍
本文档仅仅指定4.60版本的OpenGL着色语言(GLSL,OpenGL Shading Language)。其要求`__VERSION__`替代为460，并且要求`#version`仅接受460。如果`#version`指定的数字较小，则接受的语言是先前版本的着色语言，哪个版本将被支持具体取决于API中上下文的版本和类型。[引用规范](xxx)中详细讲述支持哪些语言。

先前版本的OpenGL着色语言以及OpenGL ES着色语言并不是此处版本严格意义上的子集，特别是在精度方面、名字隐藏规则、处理接口变量上。请参阅与特定语言版本相对应的规范手册，以获取该语言版本特定的详细信息。

当生成Vulkan API使用的SPIR-V时(参考[引用规范](xxx))，可以称目标为Vulkan。

尽管此规范和OpenGL规范是OpenGL着色语言的标准，但对于SPIR-V的生成，它依旧是SPIR-V的规范以及SPIR-V客户端API规范，SPIR-V客户端API是生成SPIR-V的规范。查看[引用规范](xxx)获取更多信息。

对于SPIR-V的生成，SPIR-V客户端API指定操作SPIR-V着色器的命令。

独立的离线工具链可以编译GLSL到SPIR-V中间语言。无法使用`#extension`和`#version`或者profile启用SPIR-V的生成。相反的，用于将GLSL生成SPIR-V取决于离线工具链的使用。请参阅此类工具的文档，以了解如何请求为其客户端API生成SPIR-V。

GLSL->SPIR-V编译器必须指示哪些SPIR-V功能在运行时合法，并且会为那些功能以外的GLSL功能使用提供错误。 对于与实现相关的限制也是如此，该限制可以由前端针对GLSL源中存在的内置常量进行错误检查：可以将此类限制告知前端，并在超出限制时报告错误。

SPIR-V特性不受SPIR-V功能的控制，但确实有等效的GLSL对应项（stages、内置函数、类型、限制等）仅应在支持GLSL对应项的OpenGL驱动程序上工作。

除非指定了其他profile，否则本规范中对[OpenGL规范](xxx)的所有引用为4.6版的Core profile。
