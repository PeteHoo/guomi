这个项目是原来是lpilp/guomi的国密整理，但是接入兴业银行的时候必须修改sm4的代码，为了避免修改vender包，所以我对包进行修改，其他安装的要求可以参考lpilp/guomi的要求

# php sm2 sm3 sm4 国密算法整理
* 本项目支持php版本的国密sm2的签名算法，非对称加解密算法，sm3的hash，  sm4的对称加解密，要求PHP７，打开gmp支持
* 目前如果服务器配套的使用的是openssl 1.1.1x， 目前到1.1.1.l(w) ，sm3，sm4都可以直接用openssl_xxx系列函数直接实现，不必大量的代码，不支持sm2的签名，sm2的加解密
 
## 安装

```
composer require pete-hoo/guomi
```
> 请确保你升级到 `composer 2` 及以上版本。`PHP >=7.2`,打开gmp组件支持。