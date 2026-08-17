# LaoSan NiuLai Vision

一个用于参考图风格转译的 Codex / ChatGPT Skill：将人物、动物、产品或场景重构为粗粝、抽象、原始雕塑感的乡土几何视觉，同时保留主体、构图、姿态与必要的识别特征。

> 本项目是独立创作的视觉工作流，与任何电影、片方、工作室或其他同类仓库无官方关联。

## 特点

- 先识别并锁定主体、数量、姿态、轮廓和构图，再进行风格化
- 提供 `light`、`rough`、`extreme` 三档转译强度，默认使用 `rough`
- 强调超大几何切面、硬折线、笨拙比例、粗糙哑光材质与未完成感
- 主动排除光滑皮肤、精细拓扑、干净倒角、商业动画和精美 3D 渲染感
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
选择 rough 强度，保留人物数量、姿势、轮廓和必要的五官识别点；
使用少量超大切面、硬折线和原始雕塑块面，允许比例略显笨拙；
不要光滑皮肤、精细建模、干净倒角和精美商业 3D 感。
```

如果没有指定强度，Skill 默认使用 `rough`。

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
