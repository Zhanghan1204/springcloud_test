**Jwt**  
最常见的场景为授权认证,一旦用户登录,后续每个请求都将包含Jwt,系统在每次
处理用户请求之前,都要先进行Jwt安全验证,通过之后再进行处理.  

Jwt由3部分组成,3部分用'.'(点)拼接  
header:token的类型,算法的名称  
Payload:载荷,存放有效信息的地方,分为三部分  
Signature:签名,加密之后的header+加密之后的payload,然后整体再加密  