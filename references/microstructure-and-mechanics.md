# Microstructure and mechanics: AM–HEA

用于增材制造高熵／中熵／多主元合金的组织、性能、硬化和断裂写作。
本文件给出判读与报告方法；具体组织、参数、机制和数值由当前研究提供。
语言节奏参见 [style-and-vocabulary.md](style-and-vocabulary.md)，涉及分项强化时再读 [strengthening-models.md](strengthening-models.md)。

## 1. 先确认样品与比较口径

局部润色只核对涉及的输入；新写 Methods 或跨状态 Results 时再整理完整样品表。

| 项目 | 记录内容 |
|---|---|
| 合金与原料 | 名义／实测成分及 at.%／wt.%；预合金粉、混粉或丝材；实际粒径／形貌／氧含量等已有信息 |
| 增材路线 | L-PBF、DED、WAAM 或其他实际路线；首次定义缩写，沿用目标期刊写法 |
| 工艺变量 | 所比较的功率、速度、层厚、道间距、扫描策略、预热、气氛等；按实际路线取用 |
| 热史与状态 | as-built、去应力、固溶、时效、HIP 等；温度、时长、气氛、冷却方式来自实验记录 |
| 方向与位置 | BD／构建方向、扫描／横向、观察截面、试样轴向与构建方向关系；必要时标取样高度 |
| 性能测试 | 拉伸／压缩／疲劳／断裂等实际项目；温度、应变率、几何、标距、应变获取方法 |
| 统计与对照 | 独立试样数、视场或粒子数、误差定义；铸态／打印态／热处理态及同条件基线 |

为合金代号建立唯一状态表，避免同一缩写同时表示不同参数、方向或热处理状态。
多个视场和重复压痕属于技术重复，不能无说明替代独立样品重复。
合金元素设计和工艺选择应与可检验的相、缺陷或性能问题相连。

### L-PBF 能量输入的使用

当研究采用该定义时，可记录名义体积能量密度：

\[
E_v=\frac{P}{vht}
\]

其中 P 为激光功率，v 为扫描速度，h 为道间距，t 为层厚；W、mm/s、mm、mm 对应 J/mm³。
同时保存各原始参数与扫描策略。相同 E_v 不表示熔池、缺陷或组织等效；该组合量不替代工艺与熔池物理。
本式按具体定义使用，不直接套入送丝、电弧或其他采用不同能量尺度的工艺。见外部依据 M3。

## 2. 组织叙事：按科学问题组织尺度

可选主线：

`工艺／热史 → 宏观成形与缺陷 → 相、晶粒与亚结构 → 化学分配及界面 → 性能 → 变形与损伤证据`

每段推进：

`具体图／面板 → 样品与区域 → 可见特征或统计 → 状态／相区对照 → 局部解释`

可将相鉴定先行，也可先展示最能建立主张的组织或性能。
导师样本中 P01/P04 接近 XRD→SEM→EBSD→TEM；P08 在 EBSD 前展示 TEM；P03 无独立 XRD 结果。
因此，仪器顺序不是固定章节目录；没有的数据和技术无需补成默认章节。
胞状亚结构、层片、晶粒和熔池属于不同尺度，分别命名并统计，不共用一个“grain size”。

## 3. 表征的观察、定量与解释

| 技术 | 优先报告 | 可以建立的证据 | 解释前核对 |
|---|---|---|---|
| XRD | 状态、扫描条件、峰位／索引、变化；需要时报告拟合 | 可检出的相组成、峰变化；适当条件下量化相含量或晶格参数 | 峰重叠、织构、残余应变和仪器影响；峰高不直接等于相分数 |
| OM／SEM | 截面与取样位置、低倍全貌→高倍结构、尺度和代表区域 | 熔池轮廓、胞／枝晶／层片、孔裂形貌及二维分布 | 形貌不能独立证明相身份或孔隙形成过程；统计区间和视场要明确 |
| EDS／EPMA | 元素、空间分辨率、图／点／线位置、定量方法 | 给定空间尺度的元素分配与成分差异 | 信号体积、背景和重叠；定量结论与分辨率匹配 |
| EBSD | 相别、截面、步长、索引／清洗、IPF／phase／KAM／PF 等实际图 | 晶粒、取向、织构、相分布及按明确方法得到的局部错配 | KAM 对步长／邻域／阈值敏感；总位错密度、再结晶状态不由一张颜色图自动确定 |
| TEM／SAED | 取样状态和位置、BF／DF、区轴、反射索引与相区 | 纳米组织、缺陷、有序超点、局部相与晶体学关系 | 代表性、成像条件、厚度与对比；线状对比不自动等同某类位错或层错 |
| HRTEM／FFT／IFFT | 区域、选取反射、对应关系、界面两侧结构 | 局部晶格、取向、失配位错及有序结构证据 | 图像处理影响；一致取向不自动等于完全共格或已发生滑移传递 |
| APT（如提供） | 针尖来源、重构、分割／等浓度阈值、浓度剖面及统计 | 纳米尺度化学分配、团簇／析出成分与界面偏聚 | 局部放大、检测和阈值敏感性；APT 化学证据需与晶体结构证据配合 |
| CT／其他缺陷测量 | 体素／分辨率、检测阈值、体积、孔裂尺寸和分布 | 在给定检测限内的三维缺陷统计 | 未检出不等于不存在；与二维面积分数、密度法保持各自定义 |

XRD 中 FCC／BCC 主峰与 TEM 中 L1₂／B2 有序反射应互相对应；需要结构索引时才写 confirms。
为 TEM 纳米析出统计交代半径／直径、相内体积分数、粒子数、分布与测量方法。
相对界面错配应按实际匹配晶面／晶向的周期计算，不以不同晶体结构的晶格常数直接相减替代。

### 增材制造中常见的证据连接

- **致密化／缺陷**：报告测量法和检测范围，连接实际孔裂特征与工艺变化；不从单个圆孔或不规则孔唯一判定气孔、钥孔或未熔合过程。
- **熔池与胞状亚结构**：分别描述熔池尺度和胞／枝晶尺度；冷却速率、温度梯度或 G/R 等须来自明确测量、模拟或有来源的估算。
- **各向异性**：保持观察截面、织构参考系、加载轴和 BD 对应；比较性能需要相应方向的测试，不能只由柱状晶宣布某方向更强。
- **热处理**：同时检查析出、回复／再结晶、相变、残余应力和缺陷变化中实际测到的部分，避免把全部增量归于一个显微特征。
- **损伤**：孔裂与塑性局域化的关联由位置对应、断口、原位或其他实际证据建立；最终断口提供路径线索，时间先后另需证据。

## 4. EBSD 与 TEM 的段落范式

### EBSD

先让读者知道哪张图、哪一相、哪种状态，再给粒径／相分数／取向等实际统计。
对多相或多状态，用 while／whereas／respectively 建立一一对应，最后解释与研究问题有关的差别。

> Fig. {X}(a–c) shows the [actual EBSD maps] of [states] on the [section]. Compared with [reference], [state] exhibits [measured phase-resolved difference]. The [defined quantities] are [values], respectively. [Additional evidence] indicates [supported local interpretation].

当 KAM 用来估算 GND 时，报告所选关系、步长、角度阈值与估计范围，再讨论其与直接位错／变形证据的一致性。
未经该分析时，直接写 higher KAM 或 greater local misorientation，不转换成总位错密度数值。

### TEM／界面

> Fig. {Y}(a) presents the BF-TEM image of [region and state]. [Observed defects or particles] are visible within [phase], whereas [measured difference] is observed in [comparison region]. The corresponding [SAED/HRTEM/EDS] results identify [actual structural or chemical finding]. These observations [show/indicate/suggest] [one evidence-matched consequence].

按实际证据选择观察动词和解释力度，不强制每项鉴定使用 suggests。
有直接滑移传递证据才连接到跨界面传递；只看到塞积时先报告塞积与阻碍。
图中未提供的区轴、晶面、矢量、相名和缺陷密度保留缺口，不由模板补齐。

## 5. 力学曲线：先定义再比较

### 指标与条件

记录 YS 的定义、UTS／UCS、uniform elongation／fracture elongation／compressive strain 及其实际测量方法。
保持拉伸与压缩应力／应变的符号、名称与试样定义一致；TE／FE 的含义在稿内唯一。
用数值报告增益和代价；评价 superior／excellent 时给出比较对象和相同测试条件。
文献对照至少核对温度、加载方式、方向、应变率、状态与应变指标，差异足以改变解释时在图注或正文说明。

### 工程量与真量

对于颈缩前均匀的单轴拉伸，采用相应近似时可用：

\[
\sigma_t=\sigma_e(1+e),\qquad
\varepsilon_t=\ln(1+e),\qquad
\varepsilon_p=\varepsilon_t-\sigma_t/E.
\]

e 为无量纲工程应变，σ_e 为工程应力，E 与应力同单位。
这是常用均匀拉伸分析口径；颈缩后面积、应力三轴性与变形非均匀性需另行处理。
压缩数据保留所选符号约定，并核查摩擦、鼓肚及几何处理；不把拉伸换算不加说明地套用。

### 加工硬化率

当采用塑性真应变口径时：

\[
\Theta=\mathrm{d}\sigma_t/\mathrm{d}\varepsilon_p.
\]

若原数据以真总应变求导，沿用并明确定义；两种口径不混作同一结果。
交代平滑／求导方法与区间，检查初始弹塑过渡、噪声和颈缩前后界限。
阶段数从数据确定，给出区间和趋势：快速下降、缓降／平台、回升或最终下降等。
曲线波动或平台需要与对应应变下的显微证据连接，才讨论特定孪晶、相变或位错机制。
没有中断变形实验时，区分“终态可见缺陷”与“某一阶段启动的机制”。

### 课题组式性能段

> Fig. {X}(a) shows the engineering stress–strain curves of [states] tested at [conditions]. Compared with [reference], [state] exhibits [quantified change]. Specifically, its YS, UTS and [defined elongation] are [values], respectively. Fig. {X}(b) presents the [defined hardening rate], which [measured trend over a stated interval]. This behavior is [attributed to/consistent with] [mechanism linked to actual evidence].

在未给出硬化曲线或机制证据时，省去对应句子，完成数据足够的部分。
单项较低的性能直接报告，不上升为对整项工作的笼统否定。

## 6. 断口与损伤

按 `观察位置／状态 → 低倍全貌 → 高倍特征与尺度 → 对照 → 断裂模式及组织联系` 写。

| 特征 | 报告重点 | 解释范围 |
|---|---|---|
| 韧窝／撕裂棱 | 分布、尺寸与深浅、夹杂／孔洞关联、状态差异 | 微孔聚合等解释需与形貌及组织互证，韧窝大小不直接等于断裂韧度 |
| 解理／准解理特征 | 平面、台阶、河流花样及局部韧性特征 | 支持脆性或混合模式的判断，具体相区需位置／成分证据 |
| 沿晶／穿晶路径 | 与晶界、相界、熔池边界及未熔合区的真实对应 | 几何重合先描述，起裂顺序和扩展动力学按证据决定 |
| 微裂纹与缺陷 | 位置、方向、尺度、缺陷类型及统计 | 结合局部变形、原位或断后证据讨论起裂／偏转／钝化 |

P01/P02/P04/P06/P07 的断口写法可迁移为段落节奏；P03/P08 没有必须复制的独立断口章节。
宏观强度与延伸率支持强塑性讨论；断裂韧性结论对应 K、J 或其他适当断裂测量。

## 7. 变形机制：用证据衔接尺度

| 拟议机制 | 当前稿件应提供的关键证据 |
|---|---|
| 位错滑移／储存 | 实际缺陷形态、相区与前后状态；需要密度时说明测量方法 |
| 析出相切过／绕过 | 析出结构、尺寸／间距／分数和相互作用；模型比较与实际形貌分开核对 |
| 孪晶／TWIP | 孪晶晶体学、变形状态及与硬化的联系；原有退火孪晶与变形孪晶区分 |
| TRIP | 变形前后或原位相变证据、相身份与分数；仅低 SFE 推测不替代相变观察 |
| HDI | 异质域、变形不协调与相应测量；定量应力需 LUR 等操作性定义与数据 |
| 相间应变／载荷分配 | 相分辨的应变、载荷或局部变形证据；静态相图不直接给出应力分配数值 |

选择当前问题需要的机制，串成有证据的因果段落，不把机制名逐一列成必备项。
本技能不预设所有 AM–HEA 同时具有胞状网络、L1₂、B2、TWIP、TRIP 和 HDI。

## 8. 来源与适用范围

P01–P08 为用户提供的课题组样文，完整 DOI 索引见 [风格库](style-and-vocabulary.md)。
其中的图号引导、多相比较、性能与断口节奏用于文风迁移；上面的 AM 输入表及证据检查是本技能的领域化写作规则。

外部原始研究只支持下列明确例证，不成为新稿默认组织或参数：

- **M1**. *Strong yet ductile nanolamellar high-entropy alloys by additive manufacturing*. Nature 608, 62–68 (2022). [DOI: 10.1038/s41586-022-04914-8](https://doi.org/10.1038/s41586-022-04914-8)。其 L-PBF 合金展示纳米层片、层级组织与变形证据的连接；不据此预填所有 AM 合金为有序 B2。
- **M2**. *Unveiling the mechanisms of strength–ductility synergy in an additively manufactured nanolamellar high-entropy alloy*. Nature Communications (2025). [DOI: 10.1038/s41467-025-64871-4](https://doi.org/10.1038/s41467-025-64871-4)。提供成分设计、纳米层片、析出与异质结构综合解释的原始实例；本文件不移植其性能数值或机制结论。
- **M3**. Scipioni Bertoli et al. *On the limitations of Volumetric Energy Density as a design parameter for Selective Laser Melting*. Materials & Design 113, 331–340 (2017). [DOI: 10.1016/j.matdes.2016.10.037](https://doi.org/10.1016/j.matdes.2016.10.037)。针对特定 316L 单道实验讨论 VED 的适用局限，支撑保留原始工艺参数这一规则；其阈值不跨材料照用。

这些文献不是目标期刊现行投稿规范。新稿引用前，核查实际使用的原文段落及其对当前主张的支持。
