# BitMap
## 类库说明
一个基于文件的BitMap类库，通过文件指针和位运算操作，所以setBit()和getBit()执行效率还不错，BitCount()需要对二进制数据进行解包，执行时长与BitMap位数成正比

---

## 使用示例
```
$bitmap = new bitmap('/dev/shm/bitmap.bin');
$bitmap->setBit(100, 1);
echo $bitmap->getBit(100);
```