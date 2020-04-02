---
title: 可设置全屏显示的 Splashscreen
description: Control the splash screen for your app.
---
<!--
# license: Licensed to the Apache Software Foundation (ASF) under one
#         or more contributor license agreements.  See the NOTICE file
#         distributed with this work for additional information
#         regarding copyright ownership.  The ASF licenses this file
#         to you under the Apache License, Version 2.0 (the
#         "License"); you may not use this file except in compliance
#         with the License.  You may obtain a copy of the License at
#
#           http://www.apache.org/licenses/LICENSE-2.0
#
#         Unless required by applicable law or agreed to in writing,
#         software distributed under the License is distributed on an
#         "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
#         KIND, either express or implied.  See the License for the
#         specific language governing permissions and limitations
#         under the License.
-->

# cordova-plugin-splashscreen

在 [cordova-plugin-splashscreen](https://github.com/apache/cordova-plugin-splashscreen.git) 的基础上添加了全屏设置,处理了android启动app时黑屏的问题

- [Installation](#installation)
- [Preferences](#preferences)
  * [config.xml](#configxml)
- [Other](#other)

## Installation

    // 安装前请先卸载 cordova-plugin-splashscreen 插件
    cordova plugin rm cordova-plugin-splashscreen

    // 安装插件
    cordova plugin add https://github.com/shuto-cn/cordova-plugin-splashscreen.git

## Preferences

### config.xml

- `SplashFullScreen` (boolean, default to `true`). 在app未设置全屏的情况下FadeSplash是否全屏显示

    ```xml
    <preference name="SplashFullScreen" value="true" />
    ```
## Other

- 关于android启动黑屏 请保持`SplashScreen`参数值为`screen`否则请修改`src/android/res/values/style.xml`中对应资源id
- 其他配置及插件使用方法请移步[cordova-plugin-splashscreen](https://github.com/apache/cordova-plugin-splashscreen.git)