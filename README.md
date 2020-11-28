# CTDSystem_Unity
Configurable table data system for unity

## 特点
- 先每个表动态计算出bucket大小，索引放在每个bucket当中。索引与bucket的映射尽量简单，只使用少量计算。
- C语言实现，C#，lua做接口
- 表格描述文件
- 访问类型，两种:可索引随机访问，流式
- 更新: 可热更，同一表可增量更新，使用二进制diff原理
- 表中字符串收集，使用一个hash或id替换，最终生成字符串表。可作多语言使用。
