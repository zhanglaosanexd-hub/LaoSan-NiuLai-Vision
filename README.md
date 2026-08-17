# LaoSan NiuLai Vision

一个用于参考图风格转译的 Codex / ChatGPT Skill：将人物、动物、产品或场景转化为原创的低多边形乡土电影视觉，同时尽量保留主体、构图、姿态与关键识别特征。

> 本项目是独立创作的视觉工作流，与任何电影、片方、工作室或其他同类仓库无官方关联。

## 特点

- 先识别并锁定主体、数量、姿态、轮廓和构图，再进行风格化
- 提供 `light`、`balanced`、`bold` 三档转译强度
- 使用大块几何切面、克制的土地色系、哑光材质与电影化光影
- 针对“太暗、太粗糙、不像原图、背景抢主体”等常见问题提供定向修正
- 不依赖单一电影名称或创作者名称来完成提示词

## 安装

将仓库克隆或下载到你的 Skill 目录：

```bash
git clone https://github.com/zhanglaosanexd-hub/LaoSan-NiuLai-Vision.git
```

也可以下载 ZIP 后，将文件夹放入支持 Skills 的客户端目录中。

## 使用示例

```text
使用 $laosan-niulai-vision 转译这张图片。
选择 balanced 强度，保留人物数量、五官特征、姿势和原始构图；
整体不要太暗，皮肤切面细腻一些，背景简化为有雾气的乡野空间。
```

如果没有指定强度，Skill 默认使用 `balanced`。

## 目录

```text
LaoSan-NiuLai-Vision/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── style-system.md
```

## 使用边界

- 生成式编辑无法保证产品文字、Logo 或微小图案像素级不变；这类需求建议结合后期合成。
- 请勿用于移除水印、冒充官方素材或复制其他创作者的具体作品。
- 上传和使用图片时，请确保你拥有相应权利或授权。

## License

本项目采用 [MIT License](LICENSE)。
