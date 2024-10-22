---
layout:       post
title:        "2024级第2次授课 点灯"
author:       "贾昊泽"
header-style: text
catalog:      true
tags:
    - 2024
    - 新生
    - 授课
---


## 教学内容

了解并使用循环

了解并使用GPIO


## 实现功能

### 目标

| 状态 | 含义 | 灯 | 时间|
| :-: | :-: | :-: | :-: |
| 准备 | WiFi初始化         | 灯常亮 | 2s |
| 工作 | Wifi正在连接(快闪)  | 灯闪烁 | 2s |
| 完成 | WiFi连接成功       | 灯常亮 | 2s |

### 实现逻辑

```c
//1 step
//2 step

int i=0;
while(i<10){
i=i+1;//i+=1;i++;

}
for()
```

### 实现代码

```arduino
void setup() {
  // put your setup code here, to run once:
  pinMode(LED_BUILTIN, OUTPUT);
  
  //Step 1
  digitalWrite(LED_BUILTIN, 1);
  delay(2000);
  digitalWrite(LED_BUILTIN, 0);
  
  //Step 2
  for (int i=0; i<10; i++){
    digitalWrite(LED_BUILTIN,1);
    delay(100);
    digitalWrite(LED_BUILTIN,0);
    delay(100);
  }

  //Step 3
  digitalWrite(LED_BUILTIN, 1);
  delay(2000);
  digitalWrite(LED_BUILTIN, 0);

}

void loop() {
  // put your main code here, to run repeatedly:
}

```
