# Photo to Naive Illustration

把照片转成 **粗黑手绘线、极简造型、明快纯色色块** 的童趣插画。

这个 Agent Skill 整理自实际照片转绘工作流：保留主体、动作和照片里的趣味，允许删减杂物、调整元素比例、重组布局。适用于人物、静物、食物和风景。

## 效果示例

| 冰水玻璃杯 | 笑脸花朵气球 | 晾在绳上的煎蛋 |
| --- | --- | --- |
| ![玻璃杯](iced-glass.png) | ![气球](flower-balloon.png) | ![煎蛋](hanging-egg.png) |

这些生成的示例也作为 Skill 内置的风格参考。仓库不包含原作者参考作品或用户原始照片。

## 使用条件

需要支持 `SKILL.md` 技能格式、图片输入，并且有图片生成或编辑工具的 AI 助手。Skill 是供助手执行的工作说明，不包含图像模型、API 密钥或独立上传网页。GitHub 负责分发文件，不会直接替访客生图；生成权限、费用和速度由所用平台决定，结果会随模型变化。

## 一句话安装到 Codex

把下面这句话发给 Codex 即可：

```text
帮我安装这个 Skill：https://github.com/YiShne/photo-to-naive-illustration
```

仓库根目录就是完整 Skill，包含 `SKILL.md`、`prompt-recipes.md` 和三张参考图。Codex 可使用内置 skill-installer 直接从 GitHub 安装，无需手动下载或解压。安装后下一轮对话即可使用。

给安装助手的说明：本仓库 Skill 路径为 `.`，安装名称为 `photo-to-naive-illustration`。使用内置安装器时传入：

```text
--repo YiShne/photo-to-naive-illustration --path . --name photo-to-naive-illustration
```

也保留了 [完整 ZIP 安装包](photo-to-naive-illustration-github.zip)，供需要手动复制文件的使用者选择。

## 使用方式

上传照片并输入：

```text
使用 $photo-to-naive-illustration 把这张照片转成插画。
```

删减杂物、调整元素比例和优化构图已内置为默认规则，无需用户额外说明。

可继续提出：“更简单一点”“主体大一点”“保留这副眼镜”“蓝色背景换成奶油色”。后续在同一转绘对话里直接发新照片，也可以继续处理。

默认不添加文字、签名或水印，不给普通物件擅自添加笑脸；原照片上已有的笑脸等核心特征会保留。画面以少量纯色和黑色描边为目标，若模型带入明暗或纹理，可要求“保留构图，把所有颜色改为均匀纯色”。

## 包含什么

```text
SKILL.md              # 触发条件、风格规则、执行与检查流程
prompt-recipes.md     # 通用提示词和场景处理范例
iced-glass.png        # 风格参考：冰水玻璃杯
flower-balloon.png    # 风格参考：笑脸花朵气球
hanging-egg.png       # 风格参考：晾煎蛋
```

其他支持 Agent Skills 的工具也可以读取该文件夹；具体技能安装位置和生图能力以其宿主环境为准。没有生图工具时，助手应明确说明，并提供可用于生图的提示词。

Skill 不会自动发布、上传或收集使用者的照片。照片是否发送到模型服务、怎样保存，由使用者所用的宿主平台与生图工具决定。

## 包文件

- [完整安装包 ZIP](photo-to-naive-illustration-github.zip)：包含技能源文件、风格图片、提示词、元数据和说明。
- [Skill 格式压缩包](photo-to-naive-illustration.skill)：ZIP 容器，供支持导入该格式的工具使用；Codex 用户按上面的文件夹方式安装。

## 发布到 GitHub

本地包已经准备好上述文件。创建一个空的公开仓库后，通过 GitHub 的上传文件功能上传解压后的内容，保留目录结构；也可以将这些文件提交并推送到你自己的 Git 仓库。发布后分享仓库链接，别人下载并安装 Skill，再在有生图能力的助手里上传照片即可使用。

## License

仓库中的技能说明与提示词采用 MIT 许可证，见 [LICENSE](LICENSE)。示例插画作为风格参考提供，不表示对原始参考作品或原照片享有权利，也不包含原作者签名或品牌授权。
