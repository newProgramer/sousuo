# 添加文档

### 使用Post命令添加文档

```
./post -c core_name sample.csv  #在core_name核心下对sample.csv文件进行编制索引
```

### 使用Solr Web界面添加文档![](https://www.yiibai.com/uploads/images/201702/0402/413090250_71138.png)![](https://www.yiibai.com/uploads/images/201702/0402/281100210_82522.png)

### 使用Java Client API添加文档

```
import java.io.IOException;  

import org.apache.Solr.client.Solrj.SolrClient; 
import org.apache.Solr.client.Solrj.SolrServerException; 
import org.apache.Solr.client.Solrj.impl.HttpSolrClient; 
import org.apache.Solr.common.SolrInputDocument; 

public class AddingDocument { 
   public static void main(String args[]) throws Exception { 
      //Preparing the Solr client 
      String urlString = "http://localhost:8983/Solr/my_core"; 
      SolrClient Solr = new HttpSolrClient.Builder(urlString).build();   

      //Preparing the Solr document 
      SolrInputDocument doc = new SolrInputDocument(); 

      //Adding fields to the document 
      doc.addField("id", "003"); 
      doc.addField("name", "Rajaman"); 
      doc.addField("age","34"); 
      doc.addField("addr","vishakapatnam"); 

      //Adding the document to Solr 
      Solr.add(doc);         

      //Saving the changes 
      Solr.commit(); 
      System.out.println("Documents added"); 
   } 
}

```



