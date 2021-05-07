* TR

  Time of Repetition 重复时间

* 3T MRI / 1.5T MRI

  T代表特斯拉Tesla，指MRI中使用的磁体强度，影响成像质量
  
* 多序列 Multisequence 

  Such as：T1-weighted, T1- weighted inversion recovery, and T2-weighted fluid attenuated inversion recovery
  
* 多模态 multi-modal MR images（跟多序列应该是一个意思）

  Such as：T1-weighted, T2-weighted
- 金标准 **gold standard**

  **金标准**是指当前临床医学界公认的诊断疾病的最可靠方法。（使用**金标准**的目的就是准确区分受试对象是否为某病患者）

  机器学习领域更倾向于使用Ground truth，也可以认为__金标准__能够很好地代表Ground truth
  
- 部分容积效应 [Partial Volume Effect](https://zhuanlan.zhihu.com/p/46252046)

  一张512×512像素的磁共振图像，是把人体那一层的组织切成512×512个小立方体，采集每个小方体里的身体组织T1，T2信号的均值。这个小立方体称为体素。
  像素正方体如果刚好处在信号差异大的地方，部分容积效应就明显。
  
  如果刚好一块取到灰质和白质的交界处，那么这块的灰度值就是这部分组织的均值（即灰质和白质的均值），不灰不白，也就会导致边界模糊
  
  一个体素所采样的体积（1x1x1mm，1x1x3mm等）越小，图像质量越高，轮廓细节也就越清晰
  
  参考：<https://www.zhihu.com/question/45524247?sort=created>