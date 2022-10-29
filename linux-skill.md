- 动态实时查看日志

  > tail -f test.log
  >
  > tail -f test.log | sed '/Failed/ q'  出现Failed信息立刻停止

- 历史命令技巧
> ！！重复执行上个命令
> ！N 重复执行history中第N条命令
> ！pw 重复执行最近一次以pw开头的历史命令
> ！$ 表示最近一次命令的最后一个参数


