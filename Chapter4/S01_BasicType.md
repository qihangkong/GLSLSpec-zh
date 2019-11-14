# 4.1 基本类型
定义：基本类型是由语言的某些关键字定义的类型

OpenGl着色语言中支持如下的基本类型：  
透明类型

| 类型 | 含义 |
|-|-|
| void | 用于函数没有返回值 |
| bool | 条件类型，取值为true或者false |
| int  | 有符号的整型 |
| uint | 无符号整型 |
| float | 单精度浮点类型标量 |
| double | 双精度浮点类型标量 |
| vec2 | 二维单精度浮点向量 |
| vec3 | 三维单精度浮点向量 |
| vec4 | 四维单精度浮点向量 |
| dvec2 | 二维双精度浮点向量 |
| dvec3 | 三维双精度浮点向量 |
| dvec4 | 四维双精度浮点向量 |
| bvec2 | 二维布尔向量 |
| bvec3 | 三维布尔向量 |
| bvec4 | 四维布尔向量 |
| ivec2 | 二维有符号整型向量 |
| ivec3 | 三维有符号整型向量 |
| ivec4 | 四维有符号整型向量 |
| uvec2 | 二维无符号整型向量 |
| uvec3 | 三维无符号整型向量 |
| uvec4 | 四维无符号整型向量 |
| mat2  | 2x2 的单精度浮点矩阵 |
| mat3  | 3x3 的单精度浮点矩阵 |
| mat4  | 4x4 的单精度浮点矩阵 |
| mat2x2 | 2x2 的单精度浮点矩阵 |
| mat2x3 | 2x3 的单精度浮点矩阵 |
| mat2x4 | 2x4 的单精度浮点矩阵 |
| mat3x2 | 3x2 的单精度浮点矩阵 |
| mat3x3 | 3x3 的单精度浮点矩阵 |
| mat3x4 | 3x4 的单精度浮点矩阵 |
| mat4x2 | 4x2 的单精度浮点矩阵 |
| mat4x3 | 4x3 的单精度浮点矩阵 |
| mat4x4 | 4x4 的单精度浮点矩阵 |
| dmat2  | 2x2 的双精度浮点矩阵 |
| dmat3  | 3x3 的双精度浮点矩阵 |
| dmat4  | 4x4 的双精度浮点矩阵 |
| dmat2x2 | 2x2 的双精度浮点矩阵 |
| dmat2x3 | 2x3 的双精度浮点矩阵 |
| dmat2x4 | 2x4 的双精度浮点矩阵 |
| dmat3x2 | 3x2 的双精度浮点矩阵 |
| dmat3x3 | 3x3 的双精度浮点矩阵 |
| dmat3x4 | 3x4 的双精度浮点矩阵 |
| dmat4x2 | 4x2 的双精度浮点矩阵 |
| dmat4x3 | 4x3 的双精度浮点矩阵 |
| dmat4x4 | 4x4 的双精度浮点矩阵 |

```
Note: 下表所说"访问纹理"，"sampler*"不透明类型访问纹理，"image*"不透明类型访问图像，具有指定的类型。
```
浮点不透明类型：

| 类型 | 含义 |
|-|-|
| sampler1D <br> texture1D <br> image1D | 访问1D纹理的句柄 |
| sampler1DShadow | 访问1D深度纹理的句柄 |
| sampler1DArray <br> texture1DArray <br> image1DArray | 访问1D数组纹理的句柄 |
| sampler1DArrayShadow | 访问1D深度纹理数组的句柄 |
| sampler2D <br> texture2D <br> image2D | 访问2D纹理的句柄 |
| sampler2DShadow | 访问2D深度纹理的句柄 |
| sampler2DArray <br> texture2DArray <br> image2DArray | 访问2D数组纹理的句柄 |
| sampler2DArrayShadow | 访问2D深度纹理数组的句柄 |
| sampler2DMS <br> texture2DMS <br> image2DMS | 访问2D多重采样纹理的句柄 |
| sampler2DMSArray <br> texture2DMSArray <br> image2DMSArray | 访问2D多重采样纹理数组的句柄 |
| sampler2DRect <br> texture2DRect <br> image2DRect | 访问2D矩形纹理的句柄 |
| sampler2DRectShadow | 通过比较访问矩形纹理的句柄 |
| sampler3D <br> texture3D <br> image3D | 访问3D纹理的句柄 |
| samplerCube <br> textureCube <br> imageCube | 访问立方体映射纹理的句柄 |
| samplerCubeShadow | 通过比较访问立方体映射深度纹理的句柄 |
| samplerCubeArray <br> textureCubeArray <br> imageCubeArray | 访问立方体映射数组纹理的句柄 |
| samplerCubeArrayShadow | 通过比较访问立方体映射数组深度纹理的句柄 |
| samplerBuffer <br> textureBuffer <br> imageBuffer | 用于访问缓冲区纹理的句柄 |
| subpassinput | 用于访问浮点subpass输入的句柄 |
| subpassInputMS | 用于访问多重采样浮点 subpass 输入的句柄 |

有符号整型的不透明类型：

| 类型 | 含义 |
|-|-|
| isampler1D <br> itexture1D <br> iimage1D | 访问整型1D纹理的句柄 |
| isampler1DArray <br> itexture1DArray <br> iimage1DArray | 访问整型1D数组纹理的句柄 |
| isampler2D <br> itexture2D <br> iimage2D | 访问整型2D纹理的句柄 |
| isampler2DArray <br> itexture2DArray <br> iimage2DArray | 访问整型2D数组纹理的句柄 |
| isampler2DMS <br> itexture2DMS <br> iimage2DMS | 访问整型2D多重采样纹理的句柄 |
| isampler2DMSArray <br> itexture2DMSArray <br> iimage2DMSArray | 访问整型2D多重采样纹理数组的句柄 |
| isampler2DRect <br> itexture2DRect <br> iimage2DRect | 访问整型2D矩形纹理的句柄 |
| isampler3D <br> itexture3D <br> iimage3D | 访问整型3D纹理的句柄 |
| isamplerCube <br> itextureCube <br> iimageCube | 访问整型立方体映射纹理的句柄 |
| isamplerCubeArray <br> itextureCubeArray <br> iimageCubeArray | 访问整型立方体映射数组纹理的句柄 |
| isamplerBuffer <br> itextureBuffer <br> iimageBuffer | 用于访问整型缓冲区纹理的句柄 |
| isubpassinput | 用于访问整型subpass输入的句柄 |
| isubpassInputMS | 用于访问多重采样整型 subpass 输入的句柄 |

无符号整型的不透明类型：

| 类型 | 含义 |
|-|-|
| isampler1D <br> itexture1D <br> iimage1D | 访问无符号整型1D纹理的句柄 |
| isampler1DArray <br> itexture1DArray <br> iimage1DArray | 访问无符号整型1D数组纹理的句柄 |
| isampler2D <br> itexture2D <br> iimage2D | 访问无符号整型2D纹理的句柄 |
| isampler2DArray <br> itexture2DArray <br> iimage2DArray | 访问无符号整型2D数组纹理的句柄 |
| isampler2DMS <br> itexture2DMS <br> iimage2DMS | 访问无符号整型2D多重采样纹理的句柄 |
| isampler2DMSArray <br> itexture2DMSArray <br> iimage2DMSArray | 访问无符号整型2D多重采样纹理数组的句柄 |
| isampler2DRect <br> itexture2DRect <br> iimage2DRect | 访问无符号整型2D矩形纹理的句柄 |
| isampler3D <br> itexture3D <br> iimage3D | 访问无符号整型3D纹理的句柄 |
| isamplerCube <br> itextureCube <br> iimageCube | 访问无符号整型立方体映射纹理的句柄 |
| isamplerCubeArray <br> itextureCubeArray <br> iimageCubeArray | 访问无符号整型立方体映射数组纹理的句柄 |
| isamplerBuffer <br> itextureBuffer <br> iimageBuffer | 用于访问无符号整型缓冲区纹理的句柄 |
| atomic_uint | 用于访问无符号整数原子计数器的句柄 |
| isubpassinput | 用于访问无符号整型subpass输入的句柄 |
| isubpassInputMS | 用于访问无符号多重采样整型 subpass 输入的句柄 |

采样器不透明类型：

| 类型 | 含义 |
|-|-|
| sampler | 访问描述如何采样一幅纹理的 状态 的句柄 |
| samplerShadow | 访问描述如何采样一幅深度纹理的 状态 的句柄 |

此外，着色器可以使用数组和结构体聚合这些基本类型，以构建更复杂的类型。

没有指针类型。

本规范中，聚合表示使用结构体或者数组（Matrices和Vectors不是聚合的类型）。集合体，矩阵和向量将统称为复合体。

## 4.1.1 Void
如果函数没有返回值，必须使用void声明。函数没有默认的返回类型。void关键字不能用于其他的声明中(空格式或者函数的实际参数除外),否则会产生编译时错误。

## 4.1.2 Boolean 布尔
定义：布尔类型是指布尔标量和向量类型（bool，bvec2，bvec3，bvec4）。

为了使代码的条件执行更容易的表示，所以支持布尔类型，但是不期望硬件直接支持布尔类型的变量。真正的布尔类型仅仅保留意思为true或false中的一个值。GLSL中两个关键字true和false被用作布尔常量。声明布尔值，并可以选择初始化，如以下示例所示：
```
bool success;
bool done = false;
```
用于条件跳转的表达式（如果为for：？：，while，do-while）必须为bool类型。

## 4.1.3 Integers
## 4.1.4 Floats
## 4.1.5 Vectors
## 4.1.6 Matrices，
## 4.1.7 Opaque Types 不透明类型
定义：不透明类型是语言隐藏的内部结构的类型。

如下小节列出的不透明类型，是声明对其他实际上不透明对象访问句柄的变量。这些对象通过内置函数访问，不能通过直接读或写声明的变量来实现。这些变量仅仅只能被声明为函数参数或者uniform修饰符的变量。唯一一个可以使用内存修饰符的不透明类型是image类型。除了使用数组索引、结构体成员选择、括号以外，不透明类型的变量不允许为表达式中的操作数，如果使用会导致编译时错误。

不透明变量不能被当作左值(l-value)。因此不能用作out或inout的函数参数，也不能被赋值。这些用法都会产生编译时错误。但是不透明变量可以通过in参数传递来匹配类型以及存储修饰符。并且不能使用初始化来声明。

因为单个不透明类型声明有效地声明了两个对象，不透明句柄本身以及句柄操作的对象，所以存储修饰符和内存修饰符都有空间。存储修饰符修饰不透明句柄本身，内存修饰符修饰句柄操作的对象。

* 纹理组合采样器

纹理组合采样器类型(如sampler2D)是[基本类型](xxx)表中描述的用于访问纹理的sampler类型（不包含sampler和samplerShadow）。对于不同的纹理目标，有不同的纹理组合采样器类型如float、integer、unsigned integer数据类型。纹理的访问通过内置纹理函数完成[纹理函数](xxx)，`纹理组合采样用来指定要访问的纹理以及如何对其进行过滤`。

纹理组合的采样器类型是不透明类型，声明并具有上述不透明类型的行为。当在着色器中聚合到数组中时，只能使用动态Uniform的整数表达式对它们进行索引，否则结果会产生错误。

* Image

图像类型是不透明类型，如上面对不透明类型所述进行声明和表现。可以使用内存修饰符进一步修饰它们。当汇合到着色器中的数组时，只能使用动态Uniform的整数表达式对图像进行索引，否则结果将不确定。

Image变量可以操作1D、2D、3D图像，对应于一个绑定到图像单元的单独纹理图像的全部或者部分。对于不同的纹理目标有不同的图像类型如float、integer、unsigned integer。图像的访问必须使用与绑定到Image类型， 图像的访问必须使用与绑定到图像单元的纹理目标匹配的Image类型，或者对于3D/数组非分层绑定的图像应使用与图像层的尺寸匹配的图像类型(例如3D/2DArray/Cube/CubeArray的一层必须使用image2D，image1DArray的一层必须使用image1D，2DMSArray的一层必须使用image2DMS)。如果数据类型与图像不匹配，或者如果格式布局修饰符与图像单元类型不匹配，[OpenGL Specification](xxx)第8.25节"纹理图像的加载和存储"，图像访问的结果是不确定的，但不能包括程序终止。

`Image变量用于图像的加载，存储和图像函数中描述的原子功能`指定的图像访问。
