1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:<h1 id="h1"></h1>
    <script>
       var a='hihao';
       var b='123456';
       var c=a.concat(b);
       h1.innerHTML=c;
    </script>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:<input type="text" id="dl">
    <h2 id="h2"></h2>
    <script>
      var dl=document.getElementById('dl');
       h2.onclick=function(){
         if(dl.value.length<6){
             alert(dl.value.padStart(6,'0'));
         }else{
             alert(h2.innerHTML=dl);
         }
       }
    </script>

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:<h3 id="h3"></h3>
    <script>
       var num=9387.348;
       var inum=num.toFixed(2);
       h3.innerHTML=inum;
    </script>

4.一张图片是一个相对路径img/head/icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:<h4 id="h4"></h4>
    <img src="img/head/icon/1.jpg">
    <script>
       document.getElementById('h4').onclick=function(){
          window.open('4.html','_blank');
      }
    </script>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:<div id="div"></div>
    <script>
      	var div=document.getElementById('div');						
		var a=location.href;
        var b=a.indexOf('?');
        var s=a.substr(b+1);
        var o=decodeURI(s);
		// var o=decodeURI(a.substr(a.indexOf('?')+1));
		div.innerHTML='欢迎你'+'，'+o;
    </script>
