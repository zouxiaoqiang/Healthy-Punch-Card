# 中南大学nCov健康打卡脚本

**注意**：本代码使用Github-Actions定时运行，无需部署在服务器。

## 声明

**特此声明**：项目用于学习交流，仅用于各项无异常时打卡，如有身体不适等情况还请自行如实打卡！

## 使用

1. fork本项目到你的个人账号
   
2. 设置Secrets
   
    从Github中进入刚刚fork到你的个人账号下的本项目，依次点击上栏 【Setting】->【Security】->【Secrets】->【Actions】
    
    点击【New repository secrets】 按钮新建：

* USERNAME：中南大学学工号

* PASSWORD：信息门户密码


3. 启动定时打卡

    点击上栏【Actions】。选中 workflow ，点击【Run workflow】按钮。

4. 查看运行情况

    打开Actions页面，此时在workflows中应该出现了正在运行的工作流。
    
    当手动运行时会马上进行一次打卡，以后将会默认在每天的00:25左右进行打卡（Github Action定时任务会有20分钟左右的延时）



## 修改打卡时间

打开项目中的/.github/workflows/healthy.yml文件，修改corn中的值，注意使用UTC时间。
