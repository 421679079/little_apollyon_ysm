# Little Apollyon YSM（亚小妹）

适用于 Minecraft 模组 **Yes Steve Model（YSM）** 的“亚小妹”自定义玩家模型资源包。

本仓库保存模型的可编辑资源，包括模型、动画、动画控制器、贴图、语言文件和 Molang 初始化逻辑，不包含 Minecraft、Yes Steve Model 或其他模组本体。

## 使用方法

1. 在整合包中安装 Yes Steve Model 模组，并至少启动一次游戏。
2. 将本仓库根目录中的整个 `亚小妹` 目录复制到整合包的以下目录：

   ```text
   config\yes_steve_model\custom
   ```

   安装完成后的模型配置文件应位于：

   ```text
   config\yes_steve_model\custom\亚小妹\ysm.json
   ```

3. 进入游戏，在聊天栏输入以下指令重新加载 YSM 模型：

   ```mcfunction
   /ysm model reload
   ```

4. 重载完成后，即可在 Yes Steve Model 中使用“亚小妹”模型。

更新模型时，直接使用新版本的 `亚小妹` 目录覆盖旧目录，再次执行 `/ysm model reload` 即可。

## 仓库结构

```text
亚小妹/
├─ ysm.json       # YSM 模型入口与元数据
├─ models/        # 玩家、手臂、载具和投射物模型
├─ animations/    # 主动画与兼容动画
├─ controller/    # 动画控制器
├─ textures/      # 模型及界面贴图
├─ functions/     # Molang 初始化逻辑
├─ lang/          # 中文和英文文本
└─ avatar/        # 作者头像资源
```

本项目不需要编译。修改资源后，可将 `亚小妹` 目录直接放入 YSM 的 `custom` 目录进行测试。

## 作者与原作品

- 作者：東葉月
- 原作者：4911
- 原作品：[哔哩哔哩 BV1GSoUBYEK7](https://www.bilibili.com/video/BV1GSoUBYEK7)

作者信息以模型内的 `ysm.json` 元数据为准。

## 许可证

除非具体文件另有说明，本仓库内容以 [GNU General Public License v3.0](LICENSE) 发布。

