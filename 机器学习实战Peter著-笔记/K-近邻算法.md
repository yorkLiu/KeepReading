<script type="text/javascript" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML"> </script>
formula1: $$n==x$$

formula2: $$n!=x$$

formula3: (m==y)

formula4: [m!=y]

formula5: \(k==z\)

formula6: \[k!=z\]

# K-近邻算法 (KNN)
> K-近邻算法 (KNN)工作原理: 存在一个样本数据集合，也称作训练样本集，并且样本集中每个数据都存在标签，即我们知道样本集中第一数据与所属分类的对应关系。输入并没有标签的新数据后，将新的数据每个特征与样本集中数据对应的特征进行比较，然后算法提取样本集中特征相似数据(最近邻)的分类标签。一般来说，我们只选择样本数据休中前k个最相似的数据，这就是k-近邻算法的出处，通常k是不大于20的整数。

* 优点: 精度高，对异常值不敏感，无数据输入假定
* 缺点: 计算复杂度高，空间复杂度高
* 适用数据范围: 数值型和标称型

## 距离计算公式
* 1.欧氏距离公式, 计算两个向量点 xA和xB之间的距离
   * <a href="https://www.codecogs.com/eqnedit.php?latex=\sqrt{(xA_0&space;-&space;xB_0)^{2}&space;&plus;&space;(xA_1&space;-&space;xB_1)^{2}}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sqrt{(xA_0&space;-&space;xB_0)^{2}&space;&plus;&space;(xA_1&space;-&space;xB_1)^{2}}" title="\sqrt{(xA_0 - xB_0)^{2} + (xA_1 - xB_1)^{2}}" /></a>
   * I.E: 点 （0,0）与 (1,2)之间的距离为:
      * $$\sqrt{(1-0)^{2} + (2-0)^{2}}$$
   * 点(1,0,0,1) 与 (7,6,9,4)之间的距离为:
      * $$ \sqrt{(7-1)^{2} - (6-0)^{2} - (9-0)^{2} - (4-1)^{2}} $$
      * Let $\text{S}_1(N) = \sum_{p=1}^N \text{E}(p)$
      * "Let $\text{S}1(N) = \sum{p=1}^N \text{E}(p)$"

* 2.
