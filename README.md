# TMDB-Movie-EDA
EDA for TMDB movies

本项目是对TMDB（The Movie Database）上的电影信息进行探索性分析。试图分析电影行业产量质量发展趋势，从电影投资人角度分析如何提高影片的票房，利润和口碑，找到流行趋势。 
报告分为四部分： 一.提出问题 二.清洗数据 三.分析数据 四.总结
项目难点在于清洗数据：
1）含有大量json格式的数据，需要将他们解码成Python数据类型。
2）对类型变量进行one－hot编码处理，为每一个类别引入一个新特征。

数据来源：https://www.kaggle.com/tmdb/tmdb-movie-metadata

Jupyter Notebook中含有每一部分结合代码的具体解释。
