# vue中import的css是全局scoped无效
---
**解决方案**

```
<style src="./index.css" scoped="scoped">

</style>
```
改用src的方式