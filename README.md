# BitMap
## 类库说明
这是一个基于文件的PHP BitMap类库，通过使用文件指针和位运算操作BitMap，所以setBit和getBit执行效率还不错，但是BitCount方法需要对二进制数据进行解包，Bitmap位数特长的时候算法耗时会很久

---

## 使用示例
```
$bitmap = new bitmap('/dev/shm/bitmap.bin');
$bitmap->setBit(100, 1);
echo $bitmap->getBit(100);
```