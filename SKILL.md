# Avatar Helper 🦞

让 AI 帮你生成专属头像的提示词，配合壁纸画廊网站使用。

## 触发词
- 帮我生成头像
- 做头像
- 头像 prompt
- 下载头像
- 帮我挑头像

## 功能

### 1. 生成头像描述
根据用户的特征描述，生成适合 DIY 卡通头像生成器的英文提示词

**示例：**
- 用户："帮我做一个可爱的小龙虾头像"
- 输出：`Cute little lobster, red shell, big round eyes, smiling face, wearing a small hat, orange background, cartoon style`

### 2. 风格建议
提供多种风格选择：
- 卡通 (Cartoon)
- 动漫 (Anime)
- 简约 (Minimalist)
- 复古 (Vintage)
- 赛博朋克 (Cyberpunk)
- 水彩 (Watercolor)
- 像素 (Pixel Art)

### 3. 特征提取
从用户描述中提取关键特征：
- 发型（双马尾、短发、长发、卷发等）
- 眼睛颜色
- 服装风格
- 配饰（眼镜、帽子等）
- 表情

### 4. 下载头像到本地
支持两种方式下载头像：

**方式一：从网站下载**
当用户指定了想要的头像时，可以帮用户下载到 `workspace/assets/avatar.jpg`

**方式二：自定义头像生成器**
支持自定义头像生成器 URL，默认使用：https://wallpaper.dfyx.click/avatar

## 使用流程

1. **描述你想要的头像**
   - "帮我做一个金色双马尾的女孩"
   - "想要一个酷酷的男生头像"

2. **AI 生成提示词**
   - 将描述转换为英文提示词

3. **生成或选择头像**
   - 打开 https://wallpaper.dfyx.click/avatar
   - 使用生成的提示词，或直接浏览挑选

4. **下载保存**（可选）
   - 告诉 AI 你喜欢哪个，帮你下载到本地

## 输出格式
- 头像提示词：返回适合输入到 DIY 头像生成器的英文描述
- 下载操作：使用浏览器工具从网站下载图片到 workspace/assets/
