# LaoSan NiuLai Vision

一个用于参考图风格转译的 Codex / ChatGPT Skill：将人物、动物、产品或场景重构为带有乡野舞台感的低成本 CGI 画面，同时保留主体、构图、姿态与关键识别特征。

> 本项目是独立创作的视觉工作流，与任何电影、片方、工作室或其他同类仓库无官方关联。

## 特点

- 先锁定主体数量、姿态、轮廓、构图和 3–5 个识别锚点
- 提供 `light`、`scene`、`uncanny` 三档强度，默认使用 `scene`
- 以低顶点圆钝模型、早期平滑着色、低分辨率拉伸贴图、僵硬绑定和扁平光照制造粗粝感
- 将背景简化为重复树木、平面地面、渐变天空等朴素舞台布景
- 主动排除泥塑石雕、精致低模、真实毛发、PBR 材质和商业动画质感
- 按模型、贴图、绑定、光线、环境、画面完成度六层进行定向修正

## 安装

```bash
git clone https://github.com/zhanglaosanexd-hub/LaoSan-NiuLaiVision-Skill.git
```

也可以下载 ZIP 后，将文件夹放入支持 Skills 的客户端目录中。

## 使用示例

```text
使用 $laosan-niulai-vision 转译这张图片。
选择 scene 强度，保留主体数量、姿势、构图、配色和关键识别点；
使用低顶点圆钝模型和早期平滑着色，配合略显失真的比例、低分辨率拉伸贴图、僵硬眼神与扁平光照；
背景简化为朴素的乡野舞台布景，不要泥塑、精致低模或商业动画感。
```

如果没有指定强度，Skill 默认使用 `scene`。

## 目录

```text
LaoSan-NiuLaiVision-Skill/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── style-system.md
```

## 使用边界

- 生成式编辑无法保证产品文字、Logo 或微小图案像素级不变；这类需求建议结合后期合成。
- 本 Skill 只抽象可复用的视觉结构，不复刻具体电影镜头、角色、对白或字幕。
- 请勿用于移除水印、冒充官方素材或复制其他创作者的具体作品。
- 上传和使用图片时，请确保你拥有相应权利或授权。

## License

本项目采用 [MIT License](LICENSE)。
