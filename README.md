# testpflag

[github repo](https://github.com/spf13/pflag)

[参考网址](https://o-my-chenjian.com/2017/09/20/Using-Flag-And-Pflag-With-Golang/)


````shell
git rm -r  --cached ".idea"

go build example_flag.go
./example_flag -h

./example_flag chenjian

args=[chenjian], num=1
arg[0]=chenjian
name= CHENJIAN
age= 27
gender= female
flagname= 1234


./example_flag -name balbalba -age 1111 -flagname=12333 dfdf xccccc eette
args=[dfdf xccccc eette], num=3
arg[0]=dfdf
arg[1]=xccccc
arg[2]=eette
name= balbalba
age= 1111
gender= female
flagname= 12333

./example_flag -age=12 -name=chengwu
args=[], num=0
name= chengwu
age= 12
gender= female
flagname= 1234

````


[git rm](https://my.oschina.net/dlpinghailinfeng/blog/388606)


- flag
- pflag

flag命令行语法
-flag XX
--flag XX
-flag=XX
--flag=XXX

pflag命令行语法
     --flag    // 布尔flags, 或者非必须选项默认值
     --flag x  // 只对于没有默认值的flags
     --flag=x
--flag 
--flag XX
--flag=XX

GNU Argument Syntax

https://www.gnu.org/software/libc/manual/html_node/Argument-Syntax.html

```shell
go test github.com/spf13/pflag
```

[pflag doc](https://godoc.org/github.com/spf13/pflag)
