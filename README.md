# Coroutines
![image](https://github.com/Papeone/Coroutines/raw/master/image/coroutines.jpg)
## 更新日志
### 8月24号
    优化代码： 
        1. 添加合理的线程池 为协程作为上下文 
        2. 将协程函数标记为内联函数提高性能

## kotlin 协程封装计划安排

        1.  顺序执行 task1，task2
        2. 并发执行 task1，task2
        3. 等待执行 task2 需等待 task1执行完毕后执行
        4. 延迟执行 task1 需要10秒之后执行
        5. 心跳执行 异步任务按指定间隔执行 Task 
        6. 任务执行感知生命周期，可以跟随当前activity的生命周期结束而自动结束，并可以配置是否在重新打开activity时是否要重新执行
        7. 任务执行可选主线程还是子线程
        8. 任务执行可以选择 需要网络或者不需要网络
        9. 任务执行可以选择网络制式4G 或者wifi下执行（5.0以上特性）
        10.任务可以选择在充电时执行（5.0以上特性）
        11. 任务执行可以随时取消，可以取消所有当前任务

## 项目介绍地址
http://www.jianshu.com/p/5986ca746bd5
