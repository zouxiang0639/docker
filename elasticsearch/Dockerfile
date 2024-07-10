FROM docker.elastic.co/elasticsearch/elasticsearch:8.9.0

# 设置环境变量
ENV ES_HOME /usr/share/elasticsearch
ENV ES_PLUGIN_DIR $ES_HOME/plugins

## 安装 IK 分词器
#RUN mkdir -p $ES_PLUGIN_DIR/ik \
#    && cd $ES_PLUGIN_DIR/ik \
#    && curl -L -O https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v8.9.0/elasticsearch-analysis-ik-8.9.0.zip \
#    && unzip elasticsearch-analysis-ik-8.9.0.zip \
#    && rm elasticsearch-analysis-ik-8.9.0.zip
#
### 添加自定义词典和停用词文件
#COPY config/custom_dict.txt $ES_PLUGIN_DIR/ik/config/custom_dict.txt
#COPY config/stopwords.txt $ES_PLUGIN_DIR/ik/config/stopwords.txt
#COPY config/IKAnalyzer.cfg.xml $ES_PLUGIN_DIR/ik/config/IKAnalyzer.cfg.xml