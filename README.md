# ajax_review
## ajax js中的ajax套路四步走



```javascript        
             // 第一步 创建一个xhr对象
            var xhr = new XMLHttpRequest();
            //第二步 判断接受状态并进行处理
            xhr.onreadystatechange = function(){
                if(xhr.readyState ==4){
                    // 接收文件做啥？
                    a.innerHTML =  xhr.responseText;
                }
            }
            //第三步创建请求，请求方式true为异步请求
            xhr.open("get","a.txt", true);
            //第四部，发送请求 ，get请求没报文则写空
            xhr.send(null)
```