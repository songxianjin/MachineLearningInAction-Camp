## 瑞丰  
过拟合指模型学习的太好了，即模型的出错容忍能力太低。因此，要降低惩罚系数C，来提高出错能力。但c也不能过小，会出现欠拟合，因此要根据实际情况调整C。

## 谁家那小谁  
SVM模型有两个非常重要的参数C与gamma。其中 C是惩罚系数，即对误差的宽容度。c越高，说明越不能容忍出现误差,容易过拟合。C越小，容易欠拟合。C过大或过小，泛化能力变差。所以c不能太大也不能太小！但是c偏小可以防止过逆和

## 安振宇  
c越高，说明越不能容忍出现误差,容易过拟合。C越小，容易欠拟合。因此，为了防止过拟合，C可以适当放小点。

## 九桢望乡  
参数c与之前正则化参数lambda相反,防止过拟合，即高方差，参数c应该减小

## 太阳老公  
SVM中参数C是惩罚系数，即对误差的容忍度。C越高表明越不能容忍误差,易过拟合。因此，为避免过拟合，应减小C值。

## ZengTudou 
C是惩罚参数，C值较大时，是对误分类的惩罚增大，C较小时是对误分类的惩罚减小。为了防止SVM过拟合，也就是学习的太好了，把数据集自身的特征当做一般特征了，应该使得C的值减小。我们假设数据集是二维的，利用SVM寻找一条线来分割数据，但是数据不完全线性可分，如果出现过拟合，得到的线应该是曲线，而减小C就会使得线更直接直线，从而减小过拟合。

## 毛蛋蛋球儿 
为防止过拟合，C应该尽量越小越好，C可以理解为松弛边界，C等于无穷时，可以理解为无松弛，即全部分类都正确。相反C越小，就表示允许分错的数量越多。


## 陈强 
参数C可以理解为调节优化方向中间隔大小与分类准确度两个指标的偏好权重。比如soft-margin SVM增加margin大小，将一些分错的点当作噪声处理，本质上就是间隔大小和噪声容忍度的一种trade-off，至于具体怎么trade-off，对哪个指标要求更高，那就体现在参数C上。

## exquisite 
惩罚系数C越高，说明越不能容忍出现误差，容易过拟合。C越小，容易欠拟合。C过大或过小，泛化能力变差，因此要根据实际数据适当调整C。

## PoleToWin 
SVM产生过拟合的原因异常数据点被选为支持向量，导致超平面被异常数据点影响，过拟合训练集解决的方法引入松弛变量和惩罚参数C。C越大，对分类错误的惩罚越大，导致过拟合严重。

## 脸红因为风太烫 
C越大表示惩罚越大，越不能容忍错误，容易造成过拟合，C越小与之相反，容易造成欠拟合 。
C一般先选1，然后0.1,0.5，10等数字

## JaAson 
异常数据点被选为支持向量，导致超平面被异常数据点影响，过拟合训练集解决的方法引入松弛变量和惩罚参数C。C越大，对分类错误的惩罚越大，导致过拟合严重。因此，在交叉验证集上，选择较小的C，对分类错误的容忍越强，减少过拟合。

