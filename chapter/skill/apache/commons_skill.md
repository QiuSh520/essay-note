# apache.commons 技巧记录

## org.apache.commons.lang3

* RandomStringUtils 随机字符串工具类
* StringUtils 字符串工具类

  ```java
  // 拿匹配结构的后缀，返回结果 sms
  StringUtils.substringAfter("/code/sms", "/code/");

  // 那匹配结果的前缀
  // ImageCodeProcessor 类名
  // 结果：Image
  // 使用场景：只用持有者管理所有实现子类的时候，可以拿到前缀，然后根据前缀拿到相关的枚举信息
  StringUtils.substringBefore(getClass().getSimpleName(), "CodeProcessor");
  ```