package client;
import java.io.IOException;

import infm.shop.Article;
public interface ArticleClient {
	  /**
     * 添加商品信息
     *
     * @param goods 被添加的商品
     * @return 操作成功与否
     */
	 String addArticle(Article goods) throws IOException;  //商品信息添加

	 
	 
	 /**
	     * 删除商品
	     *
	     * @param id 被删除的商品 id
	     * @return 操作成功与否
	     */
	    String deleteArticle(long id) throws IOException;  //删除商品
	    
	    
	    
	    /**
	     * 查询商品名字来查询商品信息
	     *
	     * @return 返回商品信息
	     */
	    String queryArticleInfo(String goodsName) throws IOException; //查询商品信息
	    
	    
	    
	    /** 
	        * 修改商品信息
	        * 
	        * 查询商品名字来修改商品信息
	        * @return 操作成功与否
	        */
	    String modifyArticleInfo(String goodsName) throws IOException; //修改商品信息
	    
	    
	    
	    
}
