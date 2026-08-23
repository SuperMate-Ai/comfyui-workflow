# ComfyUI Workflows

SuperMate 的 ComfyUI 工作流集（MiniMax H3 系列）。

## 📦 工作流

### 1. MiniMax H3 双采样 潜空间放大（comfyui 赛事专用）

- **文件**：`MiniMax H3 双采样 潜空间放大（comfyui 赛事专用）.json`
- **能力**：MiniMax H3 图生视频 / 参考图生视频（`MiniMaxH3ReferenceToVideo`）
  - 4 路参考图输入（`ref_image_0` ~ `ref_image_3`）
  - 双采样 + `H3SigmaRefiner` 精炼
  - 潜空间放大（`MinimaxH3LatentUpscaler`）→ 高分辨率成片
  - 9:16 竖屏（`ResolutionSelector`）
- **截图**：`工作流截图.jpg`
- **提示词格式**：`@图 1` / `@图 2` / `@图 3` / `@图 4` 引用参考图；`@声音 1` 引用音频

### 2. MinimaxH3 音频驱动数字人单人加速版（片尾曲）

- **文件**：`MinimaxH3音频驱动数字人单人加速版（片尾曲）.json`
- **能力**：H3 音频驱动数字人（片尾曲场景，单人加速版）
- **截图**：`片尾曲工作流截图.jpg`

## 🔧 使用

1. 将 `.json` 拖入 ComfyUI 工作区（或用 **Load** 加载）
2. 按需替换参考图 / 音频 / 提示词
3. 在 RunningHub 平台可作为 API 工作流调用（`/openapi/v2` 端点）

## 📄 许可

Apache-2.0（参见仓库根 LICENSE 说明）。
