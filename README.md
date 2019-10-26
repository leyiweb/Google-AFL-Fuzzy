# Google-AFL-Fuzzy
Google-AFL工具的使用案例

## 目录结构

* AFL ==》 Google AFL Fuzzy工具
* test-project ==》 包含不同的测试案例（目前只有Base64测试案例）

## 使用方式

### 安装AFL
```
cd AFL
make  # 编译工具
make install # 安装工具并设置环境

afl-gcc --version # 安装成功有版本提示
```

### 测试案例

* AFL-Base64-Test 

```
cd test-project/AFL-Base64-Test 
sh clean.sh          # 清理环境
sh build-afl.sh      # 通过AFI编译器编译含有桩的代码
sh afl-fuzzy-run.sh  # 构造测试单元并执行fuzzy分析工具
```
