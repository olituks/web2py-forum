web2py-Forum 
==============  
A forum for web2py based on Massimo video for reddit clone. http://vimeo.com/album/3016728/page:1/sort:preset/format:thumbnail  

If you want you can also add a routes.py file in the web2py root folder to start autmaticaly your app and simplify the url.  

```python routers = dict(   
  BASE  = dict(
    default_application='JDR', 		
    default_controller = "default"),      
    JDR = dict(languages=['en', 'fr'], default_language='fr'), )  ```  
    
To change the mdb you need to edit the modell db.py and add the line  

```python db = DAL('mysql://<userid>:<password>@mysql.server/<userid>$<db name>') ```  

- Users authentication (Login, Logon, Signin, mail confirmation, groups) 
- Categories (creat, edit, limit modification to the moderator group) 
- Posts (creat, edit) 
- Comments in a Post 
- List of posts can be sorted 
- Post can be evaluate by +1 or -1 
- See who is online 
- Bredcrumb 
- Category subdivised by master category (creat, edit, limit modification to the moderator group) 
- Can star a post and receive by mail last change
