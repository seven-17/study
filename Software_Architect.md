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

### 序列图

![image-20250806204253332](./Software_Architect.assets/image-20250806204253332.png)

### 通信图

![image-20250806204714311](./Software_Architect.assets/image-20250806204714311.png)

### 状态图

![image-20250806205334465](./Software_Architect.assets/image-20250806205334465.png)

### 活动图

![image-20250806205955145](./Software_Architect.assets/image-20250806205955145.png)

### 构件图

一个构建可能由多个类组成。

![image-20250806212331696](./Software_Architect.assets/image-20250806212331696.png)

## UML视图

![image-20250806213105022](./Software_Architect.assets/image-20250806213105022.png)

# 设计模式

1、设计模式分类

2、设计模式应用场景

3、设计模式的图形

## 创建型设计模式

如何创造对象

<img src="./Software_Architect.assets/image-20250807234735002.png" alt="image-20250807234735002" style="zoom:80%;" />

## 结构性设计模式

<img src="./Software_Architect.assets/image-20250807234825294.png" alt="image-20250807234825294" style="zoom:80%;" />





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





