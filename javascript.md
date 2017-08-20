# 1. 모바일 기기로 접속한 경우 특정 페이지로 이동

화면단의 javascript 코드로 수행

ex)
<script language="javascript">
    var uAgent = navigator.userAgent.toLowerCase();
    var mobilePhones = new Array('iphone', 'ipod', 'ipad', 'android', 'blackberry', 'windows ce','nokia', 'webos', 'opera mini', 'sonyericsson', 'opera mobi', 'iemobile');
    for (var i = 0; i < mobilePhones.length; i++)
        if (uAgent.indexOf(mobilePhones[i]) != -1)
            document.location = "http://m.example.com";
</script>
