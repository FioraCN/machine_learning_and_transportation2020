# machine_learning_and_transportation2020
# **Project1**
本次作业选用的研究方向是“糖尿病预测”，共选用了5种算法，分别是：决策树、随机森林、逻辑斯蒂回归、梯度提升和k近邻算法。
# 决策树
决策树代表的是对象属性与对象值之间的一种映射关系。树中每个节点表示某个对象，而每个分叉路径则代表的某个可能的属性值，而每个叶结点则对应从根节点到该叶节点所经历的路径所表示的对象的值。
# 梯度提升
梯度提升的思想借鉴于梯度下降法，其基本原理是根据当前模型损失函数的负梯度信息来训练新加入的弱分类器，然后将训练好的弱分类器以累加的形式结合到现有模型中。
# 随机森林
随机森林是利用多个决策树对样本进行训练、分类并预测的一种算法，主要应用于回归和分类场景。在对数据进行分类的同时，还可以给出各个变量的重要性评分，评估各个变量在分类中所起的作用。随机森林中随机是核心，通过随机的选择样本、特征，降低了决策树之间的相关性。随机森林中的随机主要有两层意思，一是随机在原始训练数据中有放回的选取等量的数据作为训练样本，二是在建立决策树时，随机的选特征中选取一部分特征建立决策树。这两种随机使得各个决策树之间的相关性小，进一步提高模型的准确性。
# 逻辑斯蒂回归
LR回归是在线性回归模型的基础上，使用sigmoid函数，将线性模型的结果压缩到[0,1]之间，使其拥有概率意义。
# k近邻算法
k近邻算法的思路是：在特征空间中，如果一个样本附近的k个最近(即特征空间中最邻近)样本的大多数属于某一个类别，则该样本也属于这个类别。

# 实验过程
1. 将数据导入，存储到 data中；
2. 检查数据是否有缺失；
3. 对数据进行划分，80%的样本作为训练集，20%的样本作为测试集；
4. 分别用梯度提升，单一决策树，逻辑斯蒂回归模型，随机森林，和k近邻算法进行训练和预测；
5.通过限制决策树和随机森林的深度解决了训练集过拟合的问题，提高了训练集的准确率。通过对KNN模型进行调参，观察不同参数下的训练集和测试集准确率变化，比较找出了最佳的参数。
6. 比较几种方法训练默认状态下的准确率;
由数据得出，在“糖尿病预测”的样本中，随机森林准确率最高。

# 心得体会
通过此次机器学习的作业，我对老师上课所讲的几种机器学习的方法有了根深一层的理解，有许多上课不是很清楚的知识点，都通过此次作业，在课后进行自主学习和巩固。总的来说此次作业受益匪浅，对我之前几次课程所学习的内容有一个巩固和提高。当然，在进行实践的过程中遇到了很多的问题，我们通过资料查询以及和同学间交流，克服了这些困难。在比较五种模型测试集的准确率时，我们发现随机森林的准确率最高。但我们对其中的三个模型进行调参时，三个模型的准确率有显著的提高。但是由于没有统一的标准，无法和其他模型进行对比，希望这个问题以后能的到解决。
