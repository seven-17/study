# 计算机硬件

## 计算机硬件组成

<img src="./Software_Architect.assets/image-20250907161932038.png" alt="image-20250907161932038" style="zoom: 60%;" />

## 中央处理单元

<img src="./Software_Architect.assets/image-20250907162354708.png" alt="image-20250907162354708" style="zoom: 60%;" />

<img src="./Software_Architect.assets/image-20250907162647223.png" alt="image-20250907162647223" style="zoom:60%;" />

## 校验码*

<img src="./Software_Architect.assets/image-20250907164353441.png" alt="image-20250907164353441" style="zoom:60%;" />

<img src="./Software_Architect.assets/image-20250907170533851.png" alt="image-20250907170533851" style="zoom:60%;" />

<img src="./Software_Architect.assets/image-20250907170916094.png" alt="image-20250907170916094" style="zoom:60%;" />

## 指令系统

<img src="./Software_Architect.assets/ca73b1e3-2549-429e-b55b-1803be85008a.png" alt="ca73b1e3-2549-429e-b55b-1803be85008a" style="zoom:60%;" />

<img src="./Software_Architect.assets/874cef3b-395f-4232-a3f3-02583c424dd1.png" alt="874cef3b-395f-4232-a3f3-02583c424dd1" style="zoom:60%;" />

<img src="./Software_Architect.assets/4de630c3-40c9-433d-8265-91bd6a54d11c.png" alt="4de630c3-40c9-433d-8265-91bd6a54d11c" style="zoom:60%;" />

### 流水线*

![2a6c4b0b-6224-41bc-8eab-433138ed57fa](./Software_Architect.assets/2a6c4b0b-6224-41bc-8eab-433138ed57fa.png)

<img src="./Software_Architect.assets/f4789871-2dd3-4c87-ab7e-8a5e12a8f4a1.png" alt="f4789871-2dd3-4c87-ab7e-8a5e12a8f4a1" style="zoom:60%;" />

<img src="./Software_Architect.assets/349f10cf-6a29-46ae-a329-3c35b294f659.png" alt="349f10cf-6a29-46ae-a329-3c35b294f659" style="zoom:60%;" />

<img src="./Software_Architect.assets/a27baece-e613-4634-aadc-b971f3027482.png" alt="a27baece-e613-4634-aadc-b971f3027482" style="zoom:60%;" />

## 存储系统

### cache

<img src="./Software_Architect.assets/38564708-9f14-4ec9-9535-2e4839a4e912.png" alt="38564708-9f14-4ec9-9535-2e4839a4e912" style="zoom:50%;" />

<img src="./Software_Architect.assets/4d931d41-716c-4764-a904-398f61e2679d.png" alt="4d931d41-716c-4764-a904-398f61e2679d" style="zoom: 60%;" />

<img src="./Software_Architect.assets/5a62ab00-bd24-487e-8b57-6a359f4aa221.png" alt="5a62ab00-bd24-487e-8b57-6a359f4aa221" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250907200913082.png" alt="image-20250907200913082" style="zoom:50%;" />

### 缓存替换算法

<img src="./Software_Architect.assets/image-20250907203417413.png" alt="image-20250907203417413" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250907203533228.png" alt="image-20250907203533228" style="zoom:50%;" />

### 磁盘

<img src="./Software_Architect.assets/image-20250907203936051.png" alt="image-20250907203936051" style="zoom:60%;" />

<img src="./Software_Architect.assets/image-20250907204759911.png" alt="image-20250907204759911" style="zoom:60%;" />

<img src="./Software_Architect.assets/image-20250907205648072.png" alt="image-20250907205648072" style="zoom:50%;" />

## 输入输出技术

<img src="./Software_Architect.assets/image-20250907205934705.png" alt="image-20250907205934705" style="zoom:60%;" />

<img src="./Software_Architect.assets/image-20250907210110449.png" alt="image-20250907210110449" style="zoom:60%;" />

## 总线

<img src="./Software_Architect.assets/image-20250907210332408.png" alt="image-20250907210332408" style="zoom:60%;" />

<img src="./Software_Architect.assets/image-20250907210610277.png" alt="image-20250907210610277" style="zoom:50%;" />

# 操作系统









# 关系数据库

## 键/候选键

<img src="./Software_Architect.assets/f7ce59667448ca02af27519822eae402.png" alt="在这里插入图片描述" style="zoom: 67%;" />

- **主属性与非主属性：组成候选键的属性就是主属性，其它就是非主属性。**

**求候选键实例**

- 将关系模式的函数依赖关系用”有向图“的方式表示。
- 找入度为0的属性，并以该属性集合为起点，尝试遍历有向图，若能正常遍历图中所有结点，则该属性集即为关系模式的候选键。
- 若入度为0的属性集不能遍历图中所有节点，则需要尝试性的将一些中间节点（既有入度，也有出度的结点）加入入度为0的属性集合中，直至该集合能遍历所有结点，集合为候选键。

<img src="./Software_Architect.assets/ac7b929e2dcf94a767076c30d4e71894.png" alt="在这里插入图片描述" style="zoom:80%;" />

## 函数依赖 Armstrong 公理

<img src="./Software_Architect.assets/image-20250806151258749.png" alt="image-20250806151258749" style="zoom: 80%;" />

<img src="./Software_Architect.assets/427a39d5195fcb94d4601a84679014f9.png" alt="在这里插入图片描述" style="zoom: 70%;" />

## 规范化理论（关系范式）

<img src="./Software_Architect.assets/03332ed2a4340f8c07df97e659c89761.png" alt="在这里插入图片描述" style="zoom:67%;" />

1. **第一范式（1NF）**：**在关系模式R中，当且仅当所有域只包含原子值，既每个属性都是不可再分的数据项，则关系模式R属于第一范式**。

   例如：以下不满足1NF，高级职称人数可以再分教授和副教授。

   <img src="./Software_Architect.assets/a388661d08a2567bd9a2015ea8501a60.png" alt="在这里插入图片描述" style="zoom:67%;" />

2. **第二范式（2NF）**：**若关系模式R ∈ 1NF，且每个非主属性完全依赖主码时（不存在部分依赖），则关系模式R属于第二范式**。

   例如：以下不满足2NF，课程号可以包含学分。

   <img src="./Software_Architect.assets/4170ec18951687974c72258edd1f78c5.png" alt="在这里插入图片描述" style="zoom:67%;" />

3. **第三范式（3NF）**：**若关系模式R ∈ 2NF，且没有非主属性对主码的传递函数依赖。则关系模式R属于第三范式**。

   例如：以下不满足3NF，系名和系位置依赖系号。

   <img src="./Software_Architect.assets/be3876a8096d9dccc8dffdd931696600.png" alt="在这里插入图片描述" style="zoom:67%;" />

4. **BC范式（BCNF）**：**设R是一个关系模式，F是它的依赖集，R属于BCNF当且仅当其F中每个依赖的决定因素必定包含R的某个候选码**。

   <img src="./Software_Architect.assets/1b0b26b1235e961d3938a8ff2665f9e3.png" alt="在这里插入图片描述" style="zoom:67%;" />



1. 

   

   







#### 软件性能测试

负载测试：测试超负荷环境中程序是否能够承担。

强度测试：在系统资源特别低的情况下考查软件系统极限运行情况。

容量测试：测试系统同时处理的在线最大用户数量。



#### 软件方法学--软件开发方法

自顶向下：将一个大问题分化成多个可以解决的小问题，然后逐一进行解决。每个问题都会有一个模块去解决它，且每个问题包括抽象步骤和具体步骤。

自底向上：根据系统功能要求，从具体的器件、逻辑部件或者相似系统开始，通过对其进行相互连接、修改和扩大，构成所要求的系统。

形式化方法：采用严格的数学方法，使用形式化规约语言来精确定义软件系统。

非形式化方法：通过自然语言、图形或表格描述软件系统的行为和特性，基于这些描述进行设计和开发。



#### arp命令

<img src="./Software_Architect.assets/image-20250806155431504.png" alt="image-20250806155431504" style="zoom: 80%;" />









# 面向对象开发

## 面向对象需求建模

<img src="./Software_Architect.assets/image-20250804220015240.png" alt="image-20250804220015240" style="zoom: 40%;" />

<img src="./Software_Architect.assets/image-20250804220509273.png" alt="image-20250804220509273" style="zoom:40%;" />

## 面向对象设计原则

<img src="./Software_Architect.assets/image-20250804220702359.png" alt="image-20250804220702359" style="zoom:40%;" />

## 面向对象测试

<img src="./Software_Architect.assets/image-20250804221637314.png" alt="image-20250804221637314" style="zoom:40%;" />

# 统一建模语言UML

![image-20250806195521623](./Software_Architect.assets/image-20250806195521623.png)

## 事物

![image-20250806192307166](./Software_Architect.assets/image-20250806192307166.png)

## 关系*

![image-20250806193541126](./Software_Architect.assets/image-20250806193541126.png)

![image-20250806194044953](./Software_Architect.assets/image-20250806194044953.png)

### 用例图

![image-20250806203322320](./Software_Architect.assets/image-20250806203322320.png)

### 序列图（顺序图、时序图）

![image-20250806204253332](./Software_Architect.assets/image-20250806204253332.png)

### 通信图（协作图）

<img src="./Software_Architect.assets/image-20250806204714311.png" alt="image-20250806204714311" style="zoom: 67%;" />

### 状态图

<img src="./Software_Architect.assets/image-20250806205334465.png" alt="image-20250806205334465" style="zoom:67%;" />

### 活动图

<img src="./Software_Architect.assets/image-20250806205955145.png" alt="image-20250806205955145" style="zoom: 67%;" />

### 构件图

一个构建可能由多个类组成。

<img src="./Software_Architect.assets/image-20250806212331696.png" alt="image-20250806212331696" style="zoom:67%;" />

## UML视图

<img src="./Software_Architect.assets/image-20250806213105022.png" alt="image-20250806213105022" style="zoom:50%;" />

# 设计模式*

1、设计模式分类

2、设计模式应用场景

3、设计模式的图形

## 创建型设计模式

如何创造对象

<img src="./Software_Architect.assets/image-20250807234735002.png" alt="image-20250807234735002" style="zoom: 50%;" />

## 结构型设计模式

描述对象和类之间的组织关系

<img src="./Software_Architect.assets/image-20250807234825294.png" alt="image-20250807234825294" style="zoom: 50%;" />

## 行为型设计模式

反映类或对象的行为

<img src="./Software_Architect.assets/image-20250808215621931.png" alt="image-20250808215621931" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250808221728609.png" alt="image-20250808221728609" style="zoom: 50%;" />

# 项目管理-进度管理

<img src="./Software_Architect.assets/image-20250808232554363.png" alt="image-20250808232554363" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250809130732323.png" alt="image-20250809130732323" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250811220247023.png" alt="image-20250811220247023" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250811221323924.png" alt="image-20250811221323924" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250811223435633.png" alt="image-20250811223435633" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250811224055210.png" alt="image-20250811224055210" style="zoom: 50%;" />

# 软件架构*

## 软件架构概述

<img src="./Software_Architect.assets/image-20250812230619956.png" alt="image-20250812230619956" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250812231029772.png" alt="image-20250812231029772" style="zoom: 50%;" />

### 软件架构设计与生命周期

<img src="./Software_Architect.assets/image-20250812232135633.png" alt="image-20250812232135633" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250812232210435.png" alt="image-20250812232210435" style="zoom: 50%;" />

### 构件技术

<img src="./Software_Architect.assets/image-20250813224044089.png" alt="image-20250813224044089" style="zoom: 40%;" />

<img src="./Software_Architect.assets/image-20250813225410862.png" alt="image-20250813225410862" style="zoom: 40%;" />

<img src="./Software_Architect.assets/image-20250813225759621.png" alt="image-20250813225759621" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250813232459700.png" alt="image-20250813232459700" style="zoom:50%;" />

## 软件架构风格

<img src="./Software_Architect.assets/image-20250814214256682.png" alt="image-20250814214256682" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250814214940049.png" alt="image-20250814214940049" style="zoom:50%;" />

### 数据流风格

<img src="./Software_Architect.assets/image-20250814215028021.png" alt="image-20250814215028021" style="zoom:50%;" />

### 调用/返回风格

<img src="./Software_Architect.assets/image-20250814222417246.png" alt="image-20250814222417246" style="zoom:50%;" />

### 独立构件风格

<img src="./Software_Architect.assets/image-20250814222925214.png" alt="image-20250814222925214" style="zoom:50%;" />

### 虚拟机风格

<img src="./Software_Architect.assets/image-20250814223257361.png" alt="image-20250814223257361" style="zoom:50%;" />

### 仓库（数据共享）风格

<img src="./Software_Architect.assets/image-20250814224311992.png" alt="image-20250814224311992" style="zoom:50%;" />

### 闭环控制

<img src="./Software_Architect.assets/image-20250814224406265.png" alt="image-20250814224406265" style="zoom:50%;" />

### C2风格

<img src="./Software_Architect.assets/image-20250814224937266.png" alt="image-20250814224937266" style="zoom:50%;" />

### 总结

<img src="./Software_Architect.assets/image-20250814225028164.png" alt="image-20250814225028164" style="zoom:67%;" />

## 层次架构风格

### C/S架构

<img src="./Software_Architect.assets/image-20250818215514820.png" alt="image-20250818215514820" style="zoom: 67%;" />

![image-20250818220719420](./Software_Architect.assets/image-20250818220719420.png)

### B/S架构

<img src="./Software_Architect.assets/image-20250818221300412.png" alt="image-20250818221300412" style="zoom:67%;" />

### RIA富互联网应用（小程序）

<img src="./Software_Architect.assets/image-20250818221805826.png" alt="image-20250818221805826" style="zoom:67%;" />

### MVC架构

<img src="./Software_Architect.assets/image-20250818222345989.png" alt="image-20250818222345989" style="zoom:67%;" />

### MVP架构

<img src="./Software_Architect.assets/image-20250818223931024.png" alt="image-20250818223931024" style="zoom:67%;" />

### MVVM

<img src="./Software_Architect.assets/image-20250818224228458.png" alt="image-20250818224228458" style="zoom:67%;" />

## 面向服务的架构风格

<img src="./Software_Architect.assets/image-20250818224310921.png" alt="image-20250818224310921" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250818232736598.png" alt="image-20250818232736598" style="zoom: 50%;" />

<img src="./Software_Architect.assets/image-20250818234102115.png" alt="image-20250818234102115" style="zoom:50%;" />

![image-20250818234341406](./Software_Architect.assets/image-20250818234341406.png)

<img src="./Software_Architect.assets/image-20250818234413343.png" alt="image-20250818234413343" style="zoom:67%;" />

<img src="./Software_Architect.assets/image-20250818235255597.png" alt="image-20250818235255597" style="zoom:67%;" />

## 软件架构复用

### 概念

![image-20250824213822570](./Software_Architect.assets/image-20250824213822570.png)

### DSSA 特定领域的软件架构

<img src="./Software_Architect.assets/image-20250825210414645.png" alt="image-20250825210414645" style="zoom:67%;" />

<img src="./Software_Architect.assets/image-20250825211331869.png" alt="image-20250825211331869" style="zoom:67%;" />

<img src="./Software_Architect.assets/image-20250825211639345.png" alt="image-20250825211639345" style="zoom:67%;" />

<img src="./Software_Architect.assets/image-20250825212036648.png" alt="image-20250825212036648" style="zoom:67%;" />

<img src="./Software_Architect.assets/image-20250825212523240.png" alt="image-20250825212523240" style="zoom:67%;" />

### ABSD 基于架构的软件开发

![image-20250825213853402](./Software_Architect.assets/image-20250825213853402.png)

<img src="./Software_Architect.assets/image-20250825215405392.png" alt="image-20250825215405392" style="zoom:33%;" />

<img src="./Software_Architect.assets/image-20250825220834596.png" alt="image-20250825220834596" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250825222122021.png" alt="image-20250825222122021" style="zoom:50%;" />

## 质量属性

### 软件系统的质量属性

![image-20250825222438762](./Software_Architect.assets/image-20250825222438762.png)

### 软件架构评估

#### 质量属性

<img src="./Software_Architect.assets/image-20250826211726100.png" alt="image-20250826211726100" style="zoom:40%;" />

<img src="./Software_Architect.assets/image-20250826215901731.png" alt="image-20250826215901731" style="zoom:40%;" />

<img src="./Software_Architect.assets/image-20250826221247512.png" alt="image-20250826221247512" style="zoom:50%;" />

#### 评估

<img src="./Software_Architect.assets/image-20250826221913278.png" alt="image-20250826221913278" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250826222000145.png" alt="image-20250826222000145" style="zoom:50%;" />

#### 基于场景的架构分析方法SAAM

![image-20250826222913960](./Software_Architect.assets/image-20250826222913960.png)

#### 架构权衡分析法ATAM*

![image-20250826224811347](./Software_Architect.assets/image-20250826224811347.png)

<img src="./Software_Architect.assets/image-20250826230726325.png" alt="image-20250826230726325" style="zoom:50%;" />

## 中间件

<img src="./Software_Architect.assets/image-20250827205807550.png" alt="image-20250827205807550" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250827210513554.png" alt="image-20250827210513554" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250827210740449.png" alt="image-20250827210740449" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250827212147231.png" alt="image-20250827212147231" style="zoom:50%;" />

# 软件可靠性

## 软件可靠性概述

<img src="./Software_Architect.assets/image-20250828213902121.png" alt="image-20250828213902121" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250828223240540.png" alt="image-20250828223240540" style="zoom:50%;" />

## 提高系统可靠性的技术

<img src="./Software_Architect.assets/image-20250828223709950.png" alt="image-20250828223709950" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250828225232245.png" alt="image-20250828225232245" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250828225448285.png" alt="image-20250828225448285" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250828225744709.png" alt="image-20250828225744709" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250828230156643.png" alt="image-20250828230156643" style="zoom:50%;" />

## 负载均衡

<img src="./Software_Architect.assets/image-20250828230905569.png" alt="image-20250828230905569" style="zoom:50%;" />

#  软件架构的演化和维护

<img src="./Software_Architect.assets/image-20250831110705552.png" alt="image-20250831110705552" style="zoom:50%;" />

## 面向对象软件架构演化

<img src="./Software_Architect.assets/image-20250831111516030.png" alt="image-20250831111516030" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250831113605747.png" alt="image-20250831113605747" style="zoom:50%;" />

## 软件架构演化方式的分类

<img src="./Software_Architect.assets/image-20250831113832506.png" alt="image-20250831113832506" style="zoom:50%;" />

### 软件架构静态演化

<img src="./Software_Architect.assets/image-20250831164634161.png" alt="image-20250831164634161" style="zoom:50%;" />

### 软件架构动态演化

<img src="./Software_Architect.assets/image-20250831172554024.png" alt="image-20250831172554024" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250831173508002.png" alt="image-20250831173508002" style="zoom:50%;" />

### 大型网站架构演化

<img src="./Software_Architect.assets/image-20250831175831854.png" alt="image-20250831175831854" style="zoom:40%;" />

<img src="./Software_Architect.assets/image-20250831180315863.png" alt="image-20250831180315863" style="zoom:50%;" />

### 软件架构维护

<img src="./Software_Architect.assets/image-20250831180803538.png" alt="image-20250831180803538" style="zoom:50%;" />

# 未来信息综合技术

## 信息物理系统（物联网）

![image-20250831181346819](./Software_Architect.assets/image-20250831181346819.png)

<img src="./Software_Architect.assets/image-20250831214914361.png" alt="image-20250831214914361" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250831215952573.png" alt="image-20250831215952573" style="zoom:50%;" />

## 人工智能

<img src="./Software_Architect.assets/image-20250831220347909.png" alt="image-20250831220347909" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250831224220373.png" alt="image-20250831224220373" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250831225337351.png" alt="image-20250831225337351" style="zoom:50%;" />

## 机器人

![image-20250901191059261](Software_Architect.assets/image-20250901191059261.png)

![image-20250901192341000](Software_Architect.assets/image-20250901192341000.png)

## 边缘计算

![image-20250901192621022](Software_Architect.assets/image-20250901192621022.png)

![image-20250901193258468](Software_Architect.assets/image-20250901193258468.png)

![image-20250901194928367](Software_Architect.assets/image-20250901194928367.png)

## 数字孪生

![image-20250901195833266](Software_Architect.assets/image-20250901195833266.png)

## 云计算

![image-20250901200345636](Software_Architect.assets/image-20250901200345636.png)

![image-20250901201117287](Software_Architect.assets/image-20250901201117287.png)

## 大数据

![image-20250901201317671](Software_Architect.assets/image-20250901201317671.png)

# 知识产权和标准化

## 知识产权定义

<img src="./Software_Architect.assets/image-20250903223029181.png" alt="image-20250903223029181" style="zoom:45%;" />

## 保护期限

<img src="./Software_Architect.assets/image-20250903224004474.png" alt="image-20250903224004474" style="zoom:45%;" />

## 知识产权人的确定

<img src="./Software_Architect.assets/image-20250903225929581.png" alt="image-20250903225929581" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250904232227539.png" alt="image-20250904232227539" style="zoom:45%;" />

## 侵权判定

<img src="./Software_Architect.assets/image-20250904232815862.png" alt="image-20250904232815862" style="zoom:45%;" />

# 数学算法

## 最小生成树

算法思想：每次找最小的边，不构成环便加入，直到找到n-1个边（n为节点数）。

```java
// 并查集-查找指定元素所属集合（带路径压缩）
int uf_find(vector<int> uf_set, int x) {
    if (uf_set[x] != x) {
        uf_set[x] = uf_find(uf_set, uf_set[x]);
    }
    return uf_set[x];
}

// 并查集-合并两个集合（将rank值低的合并到rank值高的）
void uf_union(vector<int>& uf_set, vector<int>& rank, int root1, int root2) {
    if (rank[root1] > rank[root2]) { // 若root1的rank值高于root2
        uf_set[root2] = root1; // 将root2合并到root1
    } else { // 否则（root1的rank值小于或等于root2）
        uf_set[root1] = root2; // 将root1合并到root2
        // 若root1的rank值等于root2，会导致合并后的集合rank值加1
        if (rank[root1] == rank[root2]) {
            rank[root2] ++;
        }
    }
}

int miniSpanningTree(int n, int m, vector<vector<int>>& cost) {
    for (int i = 1; i <= n; i++) { // 初始时，每个顶点（村庄）各自属于一个集合
        uf_set[i] = i;
        rank[i] = 0;
    }
    sort(cost.begin(), cost.end(), cmp); // 将cost数组按照成本价从小到大排序
    int rst = 0; // 用来累加结果
    for (int i = 0; i < cost.size(); i ++) { // 遍历cost数组
        // 查找当前边的两个顶点分别属于哪个集合
        int root1 = uf_find(uf_set, cost[i][0]);
        int root2 = uf_find(uf_set, cost[i][1]);
        if (root1 != root2) { // 若两个顶点属于不同集合
            rst += cost[i][2];
            uf_union(uf_set, rank, root1, root2); // 则合并两个集合
        } // 否则进入下一次循环
    }
    return rst;
}
```



<img src="./Software_Architect.assets/image-20250906184317892.png" alt="image-20250906184317892" style="zoom:40%;" />

## 最短路径

算法思想：维护起点A到每个节点的最短距离数组dist[n]，然后for循环，每次通过加入其他点作为中转点，看能否缩短A到其他点的最短距离。

```java
// 循环找到所有顶点的最短路径
for (int count = 0; count < V - 1; count++) {
    int u = minDistance(dist, sptSet);  // 选择距离最小的未访问顶点
    sptSet[u] = 1;  // 标记为已访问

    // 更新邻接顶点的距离
    for (int v = 0; v < V; v++) {
        // 如果邻接顶点未访问过，且起始点到u的最短距离 + u到v的距离 < 起始点到v的距离
        if (!sptSet[v] && graph[u][v] && dist[u]!= INT_MAX && dist[u] + graph[u][v] < dist[v]) {
            dist[v] = dist[u] + graph[u][v];
        }
    }
}
```

<img src="./Software_Architect.assets/image-20250906190702601.png" alt="image-20250906190702601" style="zoom:40%;" />

## 网络与最大流量

最大流量：每条线路的最小运输能力（短板）就是每条线路的最大流量。

算法思路：每次选择线路上的一条边，然后更新该线路的最大运输能力，直至没有线路能从起点到终点。

<img src="./Software_Architect.assets/image-20250906194941597.png" alt="image-20250906194941597" style="zoom:40%;" />

<img src="./Software_Architect.assets/image-20250906195718893.png" alt="image-20250906195718893" style="zoom:50%;" />

<img src="./Software_Architect.assets/image-20250906195732830.png" alt="image-20250906195732830" style="zoom:40%;" />

## 线性规划

<img src="./Software_Architect.assets/image-20250906205838905.png" alt="image-20250906205838905" style="zoom:40%;" />

<img src="./Software_Architect.assets/image-20250906205903208.png" alt="image-20250906205903208" style="zoom:45%;" />

<img src="./Software_Architect.assets/image-20250906205931925.png" alt="image-20250906205931925" style="zoom:50%;" />

## 动态规划

<img src="./Software_Architect.assets/image-20250906211906129.png" alt="image-20250906211906129" style="zoom:45%;" />

## 伏格尔法

<img src="./Software_Architect.assets/image-20250907003035653.png" alt="image-20250907003035653" style="zoom:50%;" />

## 博弈论

甲乙两人独立思考，按情况分析。

<img src="./Software_Architect.assets/image-20250907003140470.png" alt="image-20250907003140470" style="zoom:50%;" />

## 排队论

<img src="./Software_Architect.assets/image-20250907114702278.png" alt="image-20250907114702278" style="zoom:50%;" />


