1.�������ַ������ַ�������ķ������һ���ַ�,��ʾ��ҳ��idΪh1��Ԫ����
��:<h1 id="h1"></h1>
    <script>
       var a='hihao';
       var b='123456';
       var c=a.concat(b);
       h1.innerHTML=c;
    </script>

2.һ���������87��,����ƹ���д��87w,���Զ����ɴ洢870000�ķ���,��ʾ��ҳ��idΪh2��Ԫ����
��:<input type="text" id="dl">
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

3.һ������79387.348�Ĺ��̿�,������λС������,��ʾ��ҳ��idΪh3��Ԫ����
��:<h3 id="h3"></h3>
    <script>
       var num=9387.348;
       var inum=num.toFixed(2);
       h3.innerHTML=inum;
    </script>

4.һ��ͼƬ��һ�����·��img/head/icon/1.jpg,��ֻ��Ҫ�õ������ļ���Ŀ¼����ʾ��ҳ��idΪh4��Ԫ����
��:<h4 id="h4"></h4>
    <img src="img/head/icon/1.jpg">
    <script>
       document.getElementById('h4').onclick=function(){
          window.open('4.html','_blank');
      }
    </script>

5.�û�������֤��,���۴�Сд���붼����ȷ�ķ���,��ʾ��ҳ��idΪh1��Ԫ����,��ʾ��ҳ��idΪh4��Ԫ����
��:<div id="div"></div>
    <script>
      	var div=document.getElementById('div');						
		var a=location.href;
        var b=a.indexOf('?');
        var s=a.substr(b+1);
        var o=decodeURI(s);
		// var o=decodeURI(a.substr(a.indexOf('?')+1));
		div.innerHTML='��ӭ��'+'��'+o;
    </script>
