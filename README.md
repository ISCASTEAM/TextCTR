本地2w数据测试:    
# 特征工程    
**统计特征**     
> 相似度特征(各种sentence vector相似度 6dim + query单词和title句子相似度的数学统计 5dim) == 11 dim      
> 统计特征(query,title的句子&共现单词长度 7dim + 交集/并集-ngram特征 2*3 dim + 共现单词(有点冗余?)n-gram特征 4*3 dim) == 25dim     
> 统计特征(query_title位置特征 5*2 dim) = 10dim      
> 点击量特征 (query,title 点击量2dim + query下所有title的数学统计特征 6dim) = 8dim        
note:       
总共 54dim      
n-gram: 单独,连续两个,连续三个   
相似度:余弦,欧几里得,l1,l2,max(l1),min(l1)距离   
数学统计: min,max,median,acg,std,sum  

**vector特征**   
avg query - avg title

# 模型     
**GBDT**   
      
      

# 改进     
**特征方面**     
1.rank特征  
2.打压下title的点击量特征  
  
**模型方面**     
SVR...       
NN....       
....  
....  