Description:
Camaleon CMS v2.7.4 was discovered to contain a Cross Site Scripting (store XSS).

Affected Component:
All versions that are below 2.7.4

Step to reproduce :
Detection and Exploitation:
1.Go to Add Category 

2.Inject payload : "' test \<img src=\"\" onerror=\"alert(1)\"\>  to name of category and save it 

3. Go to list post and create a new post with a category that include a malicious payload. Then script is execute 

5. Go to link of post then script is execute 

poc:

![image](https://github.com/anh91/xss-camaleon-cms/assets/132877337/a16350d8-38a8-4713-84f4-99f3357696a5)

![image](https://github.com/anh91/xss-camaleon-cms/assets/132877337/70bfee2e-fed0-4e52-86f5-24d626dbccf4)

![image](https://github.com/anh91/xss-camaleon-cms/assets/132877337/522db051-3440-4178-b418-4e8f4daae3e9)


