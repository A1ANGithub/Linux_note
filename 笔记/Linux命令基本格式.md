# 命令提示符
    [root@localhost ~]#
    root：当前登录用户
    localhost：主机名
    ~：当前所在的目录，此处为“家”目录
    #：root超级用户的提示符，如果是普通用户，则为 $
## Cat
    输入命令man 1 cat可查看命令cat
    3种用法：
    1.cat  filename  一次显示一整个文件

    2.创建文件，只能创建不存在的文件
    cat > filename <<EOF或STOP
    输入文件内容
    EOF或者STOP结束输入

    3.cat  options filename
    其中options可以为
    -n 或 --number：由 1 开始对所有输出的行数编号。
    -b 或 --number-nonblank：和 -n 相似，只不过对于空白行不编号。
    -s 或 --squeeze-blank：当遇到有连续两行以上的空白行，就代换为一行的空白行。
    -v 或 --show-nonprinting：使用 ^ 和 M- 符号，除了 LFD 和 TAB 之外。
    -E 或 --show-ends : 在每行结束处显示 $。
    -T 或 --show-tabs: 将 TAB 字符显示为 ^I。
    -e : 等价于 -vE。
    -A, --show-all：等价于 -vET。
    -e：等价于"-vE"选项；
    -t：等价于"-vT"选项；

    4.合并文件
    Cat options filename1  filename2  >  filename

## 管道：
    2种用法：
    Ls | more：
    空格键：向下翻动一页
    Enter：向下翻一行
    q：离开

    Ls | less：
    空格键：向下翻动一页
    [PageDown]：向下翻动一页
    [PageUp]：向上翻动一页
    /字符串：向下查询“字符串”的功能
    ?字符串：向上查询“字符串”的功能
    n：重复前一个查询
    N：反向重复前一个查询
    q：离开