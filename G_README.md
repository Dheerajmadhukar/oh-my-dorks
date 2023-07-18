# Google Dorks for Bug Bounty

A list of Google Dorks for Bug Bounty, Web Application Security, and Pentesting

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/Dheerajmadhukar.svg?style=social&label=Follow%20%40Dheerajmadhukar)](https://twitter.com/Dheerajmadhukar)
</p>

---

### Broad domain search w/ negative search

> site:example.com -www -shop -share -ir -mfa

### PHP extension w/ parameters

> site:"example.com" intext:"php" inurl:".php?id=" OR inurl:".php?param=" OR inurl:".php?file=" OR inurl:".php?query=" OR inurl:".php?category=" OR inurl:".php?search=" OR inurl:".php?keyword=" OR inurl:".php?name=" OR inurl:".php?var=" OR inurl:".php?value=" OR inurl:".php?type=" OR inurl:".php?code=" OR inurl:".php?item=" OR inurl:".php?section=" OR inurl:".php?option=" OR inurl:".php?view=" OR inurl:".php?data=" OR inurl:".php?content=" OR inurl:".php?lang=" OR inurl:".php?config=" OR inurl:".php?template=" OR inurl:".php?ref=" OR inurl:".php?target=" OR inurl:".php?url=" OR inurl:".php?redirect=" OR inurl:".php?return=" OR inurl:".php?link=" OR inurl:".php?site=" OR inurl:".php?url=" OR inurl:".php?go=" OR inurl:".php?out=" OR inurl:".php?view=" OR inurl:".php?dir=" OR inurl:".php?pg=" OR inurl:".php?req=" OR inurl:".php?document=" OR inurl:".php?func=" OR inurl:".php?cmd=" OR inurl:".php?action=" OR inurl:".php?func=" OR inurl:".php?load=" OR inurl:".php?exec=" OR inurl:".php?execute=" OR inurl:".php?query=" OR inurl:".php?process=" OR inurl:".php?do=" OR inurl:".php?func=" OR inurl:".php?read=" OR inurl:".php?include=" OR inurl:".php?config=" OR inurl:".php?load=" OR inurl:".php?execute="

### SSRF

> site:example.com (inurl:"?data=" OR inurl:"?data_uri=" OR inurl:"?data_url=" OR inurl:"?download=" OR inurl:"?download_url=" OR inurl:"?endpoint=" OR inurl:"?external=" OR inurl:"?external_link=" OR inurl:"?external_url=" OR inurl:"?fetch=" OR inurl:"?fetch_url=" OR inurl:"?file=" OR inurl:"?file_url=" OR inurl:"?forward=" OR inurl:"?forward_url=" OR inurl:"?image=" OR inurl:"?image_source=" OR inurl:"?image_url=" OR inurl:"?link=" OR inurl:"?load=" OR inurl:"?load_url=" OR inurl:"?navigate=" OR inurl:"?out=" OR inurl:"?path=" OR inurl:"?path_to_file=" OR inurl:"?proxy=" OR inurl:"?proxy_link=" OR inurl:"?proxy_url=" OR inurl:"?read=" OR inurl:"?redirect=" OR inurl:"?redirect_url=" OR inurl:"?remote=" OR inurl:"?remote_image=" OR inurl:"?remote_image_url=" OR inurl:"?remote_url=" OR inurl:"?request=" OR inurl:"?rurl=" OR inurl:"?source_url=" OR inurl:"?src=" OR inurl:"?target=" OR inurl:"?target_path=" OR inurl:"?target_uri=" OR inurl:"?target_url=" OR inurl:"?uri=" OR inurl:"?url=" OR inurl:"?url_path=" OR inurl:"?urlto=")

### Disclosed XSS and Open Redirects

> site:openbugbounty.org inurl:reports intext:"example.com"

### Juicy Extensions

> site:"example.com" -inurl:robots.txt -inurl:sitemap.xml ext:sql OR ext:db OR ext:conf OR ext:config OR ext:log OR ext:backup OR ext:old OR ext:bak OR ext:ini OR ext:env OR ext:htaccess OR ext:passwd OR ext:txt OR ext:csv OR ext:xml OR ext:json OR ext:yml OR ext:yaml OR ext:wp-config.php OR ext:db.inc OR ext:env.inc OR ext:config.inc OR ext:ini.inc OR ext:log.inc OR ext:backup.inc OR ext:sql.inc OR ext:conf.inc OR ext:htaccess.inc OR ext:passwd.inc OR ext:key.inc OR ext:txt.inc OR ext:bak.inc OR ext:xml.inc OR ext:csv.inc OR ext:pdf.inc OR ext:ppt.inc OR ext:pptx.inc OR ext:xls.inc OR ext:xlsx.inc OR ext:md OR ext:htm OR ext:html OR ext:phps OR ext:phtml OR ext:shtm OR ext:shtml OR ext:asp OR ext:aspx OR ext:pl OR ext:cgi OR ext:cfm OR ext:cfc OR ext:rb OR ext:py OR ext:java OR ext:sh OR ext:bat OR ext:cmd OR ext:asm OR ext:c OR ext:cpp OR ext:cs OR ext:swift OR ext:vb OR ext:pas OR ext:inc OR ext:css OR ext:scss OR ext:less OR ext:js OR ext:jsx OR ext:vue OR ext:ts OR ext:tsx OR ext:coffee OR ext:go OR ext:rs OR ext:hs OR ext:fs OR ext:erl OR ext:exs OR ext:ex OR ext:clj OR ext:lua OR ext:pl OR ext:pm OR ext:tcl OR ext:ml OR ext:fsx OR ext:fsi OR ext:fsproj OR ext:h OR ext:hpp OR ext:m OR ext:mm OR ext:groovy OR ext:kt OR ext:php4 OR ext:php3 OR ext:php2 OR ext:phtml OR ext:pwml OR ext:inc OR ext:php2 OR ext:inc.php

### Code Leaks

> site:pastebin.com "example.com"

> site:jsfiddle.net "example.com"

> site:codebeautify.org "example.com"

> site:codepen.io "example.com"

### Cloud Storage

> site:s3.amazonaws.com "example.com"

> site:blob.core.windows.net "example.com"

> site:googleapis.com "example.com"

> site:drive.google.com "example.com"

> site:dev.azure.com "example[.]com"

> site:onedrive.live.com "example[.]com"

> site:digitaloceanspaces.com "example[.]com"

> site:sharepoint.com "example[.]com"

> site:s3-external-1.amazonaws.com "example[.]com"

> site:s3.dualstack.us-east-1.amazonaws.com "example[.]com"

> site:dropbox.com/s "example[.]com"

> site:box.com/s "example[.]com"

> site:docs.google.com inurl:"/d/" "example[.]com"

### XSS prone parameters

> inurl:q= | inurl:s= | inurl:search= | inurl:query= inurl:& site:example.com

### Open Redirect prone parameters

> inurl:url= | inurl:return= | inurl:next= | inurl:redir= inurl:http site:example.com

### SQLi Prone Parameters_1

> inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:example.com


> inurl:="view_items.php?id=" OR inurl:="home.php?cat=" OR inurl:="item_book.php?CAT=" OR inurl:="www/index.php?page=" OR inurl:="schule/termine.php?view=" OR inurl:="goods_detail.php?data=" OR inurl:="storemanager/contents/item.php?page_code=" OR inurl:="view_items.php?id=" OR inurl:="customer/board.htm?mode=" OR inurl:="help/com_view.html?code=" OR inurl:="n_replyboard.php?typeboard=" site:example.com

> inurl:="eng_board/view.php?T****=" OR inurl:="prev_results.php?prodID=" OR inurl:="bbs/view.php?no=" OR inurl:="gnu/?doc=" OR inurl:="zb/view.php?uid=" OR inurl:="global/product/product.php?gubun=" OR inurl:="m_view.php?ps_db=" OR inurl:="productlist.php?tid=" OR inurl:="product-list.php?id=" OR inurl:="onlinesales/product.php?product_id=" OR inurl:="garden_equipment/Fruit-Cage/product.php?pr=" site:example.com

> site:example.com inurl:="product.php?shopprodid=" OR inurl:="product_info.php?products_id=" OR inurl:="productlist.php?tid=" OR inurl:="showsub.php?id=" OR inurl:="productlist.php?fid=" OR inurl:="products.php?cat=" OR inurl:="products.php?cat=" OR inurl:="product-list.php?id=" OR inurl:="product.php?sku=" OR inurl:="store/product.php?productid=" OR inurl:="products.php?cat=" OR inurl:="productList.php?cat="

> site:example.com inurl:="product_detail.php?product_id=" OR inurl:="product.php?pid=" OR inurl:="view_items.php?id=" OR inurl:="more_details.php?id=" OR inurl:="county-facts/diary/vcsgen.php?id=" OR inurl:="idlechat/message.php?id=" OR inurl:="podcast/item.php?pid=" OR inurl:="products.php?act=" OR inurl:="details.php?prodId=" OR inurl:="socsci/events/full_details.php?id=" OR inurl:="ourblog.php?categoryid=" 

> site:example.com inurl:="mall/more.php?ProdID=" OR inurl:="archive/get.php?message_id=" OR inurl:="review/review_form.php?item_id=" OR inurl:="english/publicproducts.php?groupid=" OR inurl:="news_and_notices.php?news_id=" OR inurl:="rounds-detail.php?id=" OR inurl:="gig.php?id=" OR inurl:="board/view.php?no=" OR inurl:="index.php?modus=" OR inurl:="news_item.php?id="

> site:example.com inurl:="rss.php?cat=" OR inurl:="products/product.php?id=" OR inurl:="details.php?ProdID=" OR inurl:="els_/product/product.php?id=" OR inurl:="store/description.php?iddesc=" OR inurl:="socsci/news_items/full_story.php?id=" OR inurl:="naboard/memo.php?bd=" OR inurl:="bookmark/mybook/bookmark.php?bookPageNo=" OR inurl:="board/board.html?table=" OR inurl:="kboard/kboard.php?board=" OR inurl:="order.asp?lotid=" OR inurl:="goboard/front/board_view.php?code=" OR inurl:="bbs/bbsView.php?id=" OR inurl:="boardView.php?bbs="

> site:example.com inurl:="eng/rgboard/view.php?&bbs_id=" OR inurl:="product/product.php?cate=" OR inurl:="content.php?p=" OR inurl:="page.php?module=" OR inurl:="?pid=" OR inurl:="bookpage.php?id=" OR inurl:="cbmer/congres/page.php?LAN=" OR inurl:="content.php?id=" OR inurl:="news.php?ID=" OR inurl:="photogallery.php?id=" OR inurl:="index.php?id=" OR inurl:="product/product.php?product_no=" OR inurl:="nyheder.htm?show=" OR inurl:="book.php?ID=" OR inurl:="print.php?id=" OR inurl:="detail.php?id=" OR inurl:="book.php?id=" OR inurl:="content.php?PID=" 

> site:example.com inurl:="more_detail.php?id=" OR inurl:="content.php?id=" OR inurl:="view_items.php?id=" OR inurl:="view_author.php?id=" OR inurl:="main.php?id=" OR inurl:="english/fonction/print.php?id=" OR inurl:="magazines/adult_magazine_single_page.php?magid=" OR inurl:="product_details.php?prodid=" OR inurl:="magazines/adult_magazine_full_year.php?magid=" OR inurl:="products/card.php?prodID=" OR inurl:="catalog/product.php?cat_id=" OR inurl:="e_board/modifyform.html?code=" OR inurl:="community/calendar-event-fr.php?id=" 

> site:example.com inurl:="products.php?p=" OR inurl:="news.php?id=" OR inurl:="StoreRedirect.php?ID=" OR inurl:="subcategories.php?id=" OR inurl:="tek9.php?" OR inurl:="template.php?Action=Item&pid=" OR inurl:="topic.php?ID=" OR inurl:="tuangou.php?bookid=" OR inurl:="type.php?iType=" OR inurl:="updatebasket.php?bookid=" OR inurl:="updates.php?ID=" OR inurl:="view.php?cid=" OR inurl:="view_cart.php?title=" OR inurl:="view_detail.php?ID=" OR inurl:="viewcart.php?CartId=" OR inurl:="viewCart.php?userID=" OR inurl:="viewCat_h.php?idCategory=" OR inurl:="viewevent.php?EventID=" 

> site:example.com inurl:="viewitem.php?recor=" OR inurl:="viewPrd.php?idcategory=" OR inurl:="ViewProduct.php?misc=" OR inurl:="voteList.php?item_ID=" OR inurl:="whatsnew.php?idCategory=" OR inurl:="WsAncillary.php?ID=" OR inurl:="WsPages.php?ID=noticiasDetalle.php?xid=" OR inurl:="sitio/item.php?idcd=" OR inurl:="index.php?site=" OR inurl:="de/content.php?page_id=" OR inurl:="gallerysort.php?iid=" OR inurl:="docDetail.aspx?chnum=" OR inurl:="index.php?section=" OR inurl:="index.php?page=" OR inurl:="index.php?page=" OR inurl:="en/publications.php?id=" OR inurl:="events/detail.php?ID=" OR inurl:="forum/profile.php?id=" OR inurl:="media/pr.php?id=" OR inurl:="content.php?ID=" OR inurl:="cloudbank/detail.php?ID=" OR inurl:="pages.php?id=" OR inurl:="news.php?id=" OR inurl:="beitrag_D.php?id=" OR inurl:="content/index.php?id=" OR inurl:="index.php?i=" 

> site:example.com inurl:="?action=" OR inurl:="index.php?page=" OR inurl:="beitrag_F.php?id=" OR inurl:="index.php?pageid=" OR inurl:="page.php?modul=" OR inurl:="detail.php?id=" OR inurl:="index.php?w=" OR inurl:="index.php?modus=" OR inurl:="news.php?id=" OR inurl:="news.php?id=" OR inurl:="aktuelles/meldungen-detail.php?id=" OR inurl:="item.php?id=" OR inurl:="obio/detail.php?id=" OR inurl:="page/de/produkte/produkte.php?prodID=" OR inurl:="packages_display.php?ref=" OR inurl:="shop/index.php?cPath=" OR inurl:="modules.php?bookid=" OR inurl:="view/7/9628/1.html?reply=" OR inurl:="product_details.php?prodid=" OR inurl:="catalog/product.php?pid=" OR inurl:="rating.php?id=" OR inurl:="?page=" 

> site:example.com inurl:="catalog/main.php?cat_id=" OR inurl:="index.php?page=" OR inurl:="detail.php?prodid=" OR inurl:="products/product.php?pid=" OR inurl:="news.php?id=" OR inurl:="book_detail.php?BookID=" OR inurl:="catalog/main.php?cat_id=" OR inurl:="catalog/main.php?cat_id=" OR inurl:="default.php?cPath=" OR inurl:="catalog/main.php?cat_id=" OR inurl:="catalog/main.php?cat_id=" OR inurl:="category.php?catid=" OR inurl:="categories.php?cat=" OR inurl:="categories.php?cat=" OR inurl:="detail.php?prodID=" OR inurl:="detail.php?id=" OR inurl:="category.php?id=" OR inurl:="hm/inside.php?id=" OR inurl:="index.php?area_id=" OR inurl:="" OR inurl:="gallery.php?id=" OR inurl:="products.php?cat=" 

> site:example.com inurl:="products.php?cat=" OR inurl:="media/pr.php?id=" OR inurl:="books/book.php?proj_nr=" OR inurl:="products/card.php?prodID=" OR inurl:="general.php?id=" OR inurl:="news.php?t=" OR inurl:="usb/devices/showdev.php?id=" OR inurl:="content/detail.php?id=" OR inurl:="templet.php?acticle_id=" OR inurl:="news/news/title_show.php?id=" OR inurl:="product.php?id=" OR inurl:="index.php?url=" OR inurl:="cryolab/content.php?cid=" OR inurl:="ls.php?id=" OR inurl:="s.php?w=" OR inurl:="abroad/page.php?cid=" OR inurl:="bayer/dtnews.php?id=" OR inurl:="news/temp.php?id=" OR inurl:="index.php?url=" OR inurl:="book/bookcover.php?bookid=" OR inurl:="index.php/en/component/pvm/?view=" OR inurl:="product/list.php?pid="

> site:example.com inurl:="cats.php?cat=" OR inurl:="software_categories.php?cat_id=" OR inurl:="print.php?sid=" OR inurl:="about.php?cartID=" OR inurl:="accinfo.php?cartId=" OR inurl:="acclogin.php?cartID=" OR inurl:="add.php?bookid=" OR inurl:="add_cart.php?num=" OR inurl:="addcart.php?" OR inurl:="addItem.php" OR inurl:="add-to-cart.php?ID=" OR inurl:="addToCart.php?idProduct=" OR inurl:="addtomylist.php?ProdId=" OR inurl:="adminEditProductFields.php?intProdID=" OR inurl:="advSearch_h.php?idCategory=" OR inurl:="affiliate.php?ID=" OR inurl:="affiliate-agreement.cfm?storeid=" OR inurl:="affiliates.php?id=" OR inurl:="ancillary.php?ID=" OR inurl:="archive.php?id=" OR inurl:="article.php?id=" OR inurl:="phpx?PageID" OR inurl:="basket.php?id=" OR inurl:="Book.php?bookID=" OR inurl:="book_list.php?bookid=" OR inurl:="book_view.php?bookid=" OR inurl:="BookDetails.php?ID=" OR inurl:="browse.php?catid=" OR inurl:="browse_item_details.php" OR inurl:="Browse_Item_Details.php?Store_Id=" OR inurl:="buy.php?" OR inurl:="buy.php?bookid=" OR inurl:="bycategory.php?id=" OR inurl:="cardinfo.php?card=" OR inurl:="cart.php?action=" OR inurl:="cart.php?cart_id=" 


### SSRF Prone Parameters

> inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:example.com

### LFI Prone Parameters

> inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:example.com

### RCE Prone Parameters

> inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:example.com

### High % inurl keywords

> inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:example[.]com

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:example[.]com

### JFrog Artifactory

> site:jfrog.io "example[.]com"

### Firebase

> site:firebaseio.com "example[.]com"

### API Docs

> inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"example[.]com"

### File upload endpoints

> site:example.com ”choose file”

## Dorks that work better w/o domain

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

> site:*/security.txt "bounty"

### Apache Server Status Exposed

> site:*/server-status apache

### WordPress

> inurl:/wp-admin/admin-ajax.php

### Drupal

> intext:"Powered by" & intext:Drupal & inurl:user

### Joomla

> site:*/joomla/login

---

