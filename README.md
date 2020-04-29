![GoIndex](https://raw.githubusercontent.com/zixiwangluo/goindex/master/themes/logo.png)  
 ------------------------------
2020.4.29更新说明
1.请先fork本项目后，按下述操作进行更改，否则会出现目录空白等问题！

2.自己的git-goindex - 发布release 版本号自定，可以为1.0.6可以为其他比如 15

3.替换15行代码

原来 //cdn.jsdelivr.net/combine/gh/jquery/jquery@3.2/dist/jquery.min.js,gh/donwa/goindex@${authConfig.version}/themes/${authConfig.theme}/app.js

替换为

//cdn.jsdelivr.net/combine/gh/jquery/jquery@3.2/dist/jquery.min.js,gh/自己git名/goindex@第二步发布的release的版本号/themes/${authConfig.theme}/app.js

*注意仓库public.
-------------------------------
GoIndex  
====  
Google Drive Directory Index  
Combining the power of [Cloudflare Workers](https://workers.cloudflare.com/) and [Google Drive](https://www.google.com/drive/) will allow you to index you files on the browser on Cloudflare Workers.    

`index.js` is the content of the Workers script.  

## Demo  
material: [https://index.gd.workers.dev/](https://index.gd.workers.dev/)  
classic: [https://indexc.gd.workers.dev/](https://indexc.gd.workers.dev/)  

## Deployment  
1.Install `rclone` software locally  
2.Follow [https://rclone.org/drive/]( https://rclone.org/drive/) bind a drive  
3.Execute the command`rclone config file` to find the file `rclone.conf` path  
4.Open `rclone.conf`,find the configuration `root_folder_id` and `refresh_token`  
5.Download index.js in https://github.com/zixiwangluo/goindex and fill in root and refresh_token  
6.Deploy the code to [Cloudflare Workers](https://www.cloudflare.com/)

## Quick Deployment  
1.Open https://installen.gd.workers.dev/  
2.Auth and get the code  
3.Deploy the code to [Cloudflare Workers](https://www.cloudflare.com/)  



## About  
Cloudflare Workers allow you to write JavaScript which runs on all of Cloudflare's 150+ global data centers.  
