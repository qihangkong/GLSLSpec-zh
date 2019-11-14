# 4.3 存储修饰符
变量声明最多可以在类型的前面指定一个存储修饰符。存储修饰符可使用如下：

| 存储修饰符 | 含义 |
|-|-|
| <none:default> | local存储读/写，或者函数input参数 |
| const | 变量的值不能被改变 |
| in | 变量是由上一个着色器阶段拷贝的 |
| out | 变量拷贝到后续的着色器阶段 |
| attribute | 仅仅在兼容性的顶点着色器中，类似于顶点着色器中的in |
| uniform | 值再图元处理的过程中不会改变，链接着色器，API，和应用程序中的值 |
| varying | 兼容性，仅仅存在于vertex和fragment shader中，类似于顶点着色器中的out和片元着色器中的out |
| buffer | 值存储在buffer object中，可以被shader调用和API中读或者写 |
| shared | 仅在computer shader中，变量可以被workgroup中的work items共享 |

某些输入和输出限定变量最多可以使用一个附加辅助存储限定符限定：

| 辅助存储修饰符 | 含义 |
|-|-|
| centroid | 基于质心的插值 |
| sample | 单采样插值 |
| patch | 每个细分着色器patch属性 |
