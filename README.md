# WanWanCraft

![下载](1.png)

## 服务器详情

服务器核心：Java1.21.8 Fabric

支持BE 1.21.70 ~ 1.21.94

服务器类型：生电

地图种子：`-4914857033208116357`

JE服务器地址：`mc.classisband.xyz:37372`

BE服务器地址：`mc.classisband.xyz` 端口：`37372`

未开启正版验证

### 整合包

建议使用群内整合包以获得更好的体验

整合包使用了

CozyUI+ v1.9  作者零雾Fogg05

XeKr红显3.6  作者Xe_Kr 

整合包Mod均可删除，建议保留Music Hud

在服务器按 `M` 键可以打开点歌界面

### 网页地图

使用`Bluemap`搭建的服务器地图

`http://mc.classisband.xyz:42764`

尽量少刷新与使用，减少服务器流量开销

禁止刷流，否则关闭网页

## 指令

### EasyAuth

- `/login <password>, /l <password>`：登陆账号

- `/logout`：退出登陆

- `/register <password> <password>`：注册账号

- `/account`：管理账号

- `/unregister <password>`：注销账号

- `/changePassword <old password> <new password>`：更改密码

  **注释**： 允许玩家用以下字符组合作为密码：纯字母, 字母与下划线_, "引号与字母" 或者 "字母与&$@#"。

### 皮肤命令

**Mojang**

从有效的正版 MC 用户名获取并应用皮肤。

```minecraft
skin set mojang <用户名> [<目标玩家>]
```

**Ely.by**

从有效的 [ely.by](javascript:void(0);) 用户名获取并应用皮肤。

```minecraft
skin set ely.by <用户名> [<目标玩家>]
```

**Web**

从任何图像 URL 获取并应用皮肤。

- Steve（经典的，classic）皮肤模型

- Alex（瘦手臂，slim）皮肤模型

```minecraft
skin set web (classic|slim) "<URL>" [<目标玩家>]
```

**URL 必须有英文双引号**  目标玩家用法同上文。

> [!TIP]
>
> 如果你用Littleskin
>
> 可以直接用Littleskin直链
>
> 如“https://littleskin.cn/skinlib/show/640238”   Alex模型
>
> 那么它的直链为“https://littleskin.cn/raw/640238”
>
> 指令则为`skin set web slim "https://littleskin.cn/raw/640238" [<目标玩家>]`



- `skin refresh [<目标玩家>]`

重新获取并重新应用当前使用的皮肤。

- `skin clear [<目标玩家>]`

删除当前应用的皮肤。

- `skin reset [<目标玩家>]`

重置为默认皮肤或删除任何自定义皮肤。

### 假人指令

- `/player <name> spawn`: 在当前位置生成具有给定名称的假人玩家。
  - `... [in] <gamemode>`：在当前位置生成指定游戏模式的玩家。
  - `... [at] <position>`：在指定位置生成具有给定名称的假人玩家。
    - `... [facing] [facing]`：在指定位置生成具有给定名称，指定朝向的假人玩家。
      - `... [in] <dimension>`：在指定维度的指定位置生成具有指定名称，指定朝向的假人玩家。
        - `... [in] <gamemode>`：在指定维度的指定位置生成具有指定名称、指定朝向，指定游戏模式的假人玩家。
- `/player <name> attack [continuous | interval <ticks> | once]`: 控制玩家持续、间隔一定时间（ticks）或单次左击。
- `/player <name> use [continuous | interval <ticks> | once]`: 控制玩家持续、间隔一定时间（ticks）或单次右击。
- `/player <name> mount [anything]`: 玩家骑乘附近可骑乘的东西。
- `/player <name> dismount`: 玩家从骑乘的实体上下来。
- `/player <name> drop`: 玩家丢弃他们当前持有的物品。
- `/player <name> dropStack`: 玩家丢弃成组的物品。
- `/player <name> jump`: 玩家执行跳跃动作。
- `/player <name> kill`: 杀死玩家。
- `/player <name> look <up | down | north | south | east | west | at <x y z>>`: 玩家看向给定的方向或坐标。
- `/player <name> move <backward | forward | left | right>`: 玩家向给定的方向移动。
- `/player <name> shadow`: 使用服务器上的假玩家替换您，仅适用于服务器（不适用于单人游戏）。
- `/player <name> sneak`: 玩家执行蹲下动作。
- `player <name> unsneak`: 玩家取消蹲下动作。
- `/player <name> sprint`: 玩家开始疾跑。
- `/player <name> unsprint`: 玩家停止疾跑。
- `/player <name> stop`: 玩家停止移动并取消正在执行的所有操作。
- `/player <name> swapHands`: 玩家交换主副手的物品。
- `/player <name> turn`: 玩家转动。

### TPA类指令

- `/disposal`，`/trash` ，`/trashcan` – 打开一个临时的9x3物品栏，用于丢弃物品。屏幕关闭时内容会被删除，玩家会在聊天中收到提醒。

- `/tpa <player>`– 向另一名玩家发送传送请求。

- `/tpahere <player>`——发送请求让另一名玩家传送到你这里。

- `/tpahere`– 向所有在线玩家发送TPA请求。

- `/tpaccept <player>`——接受传送请求。

- `/tpdeny <player>`——拒绝传送请求。

- `/tpacancel`——取消你发出的传送请求。

- `/back`– 传送回你之前的位置（TPA传送后有效）。

`[target]`是可选的，默认为执行人。