# TMDB-Movie-EDA
## EDA for TMDB movies

本项目对TMDB（The Movie Database）上的电影信息进行探索性分析。试图分析电影行业产量质量发展趋势，从电影投资人角度分析如何提高影片的票房，利润和口碑，找到流行趋势。

报告分为四部分： 一.提出问题 二.清洗数据 三.分析数据 四.总结

项目难点在于清洗数据：
1）含有大量json格式的数据，需要将他们解码成Python对象。
2）对类型变量进行one－hot编码处理，为每一个类别引入一个新特征。

数据来源：https://www.kaggle.com/tmdb/tmdb-movie-metadata
tmdb_5000_credits.csv中采用的特征：
movie_id:主键电影ID
title:电影名称
cast:全体演员，在数据清洗中提炼出番位前三的演员，用三个新类别替代cast列－－actor_1,actor_2,actor_3
crew:工作组成员，在数据清洗中提炼出导演，用新类别替代crew列－－director
tmdb_5000_movies.csv中最终采用的特征：
budget:制作预算
genres:电影所属类别，一部电影通常所属多种类别，需用one-hot解码处理。
keywords:关键字
popularity:受欢迎程度
productor:制片方
countries:制作国家
release_date:上映日期
revenue:票房
duration:电影市场
status:是否上映
score:TMBD上的分数
vote_count:评分人数

Jupyter Notebook中含有每一部分结合代码的具体解释。
