# email
主要作用:
```
  当做PHP的composer使用
```
使用方法：
```
  编写composer文件 文件名为xp/email
	$smtpserver = "smtp.163.com"; //SMTP服务器
    $smtpserverport = 25; //SMTP服务器端口
    $smtpusermail = "xxxxxxxxxx@163.com"; //SMTP服务器的用户邮箱
    $smtpemailto = $to; //发送给谁
    $smtpuser = "xxxxxxx"; //SMTP服务器的用户帐号
    $smtppass = "xxxxxxx"; //SMTP服务器的用户密码
    $mailsubject = $title; //邮件主题
    $mailbody = $body; //邮件内容
    $mailtype = "HTML"; //邮件格式（HTML/TXT）,TXT为文本邮件
    $smtp = new smtp($smtpserver, $smtpserverport, true, $smtpuser, $smtppass);
    $smtp->debug = true; //是否显示发送的调试信息
    $smtp->sendmail($smtpemailto, $smtpusermail, $mailsubject, $mailbody, $mailtype);
```