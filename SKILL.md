# Avatar Helper 🦞

帮龙虾下载喜欢的头像到本地，配合壁纸画廊网站使用。

## 触发词
- 帮我挑头像
- 下载头像
- 换个头像

## 功能

### 1. 展示头像库
打开 https://wallpaper.dfyx.click/avatar 让用户挑选喜欢的头像

### 2. 下载头像到本地
当用户指定喜欢的头像后，帮用户下载到 `workspace/assets/avatar.jpg`

## 使用流程

1. **用户说**："帮我挑个头像是"

2. **AI 回应**：
   - 打开头像网站让用户挑选
   - 或直接问用户喜欢什么风格

3. **用户选择**后：
   - 告诉 AI 喜欢哪张
   - AI 用浏览器打开那张图，点击下载

4. **AI 下载**：
   - 将图片保存到 `workspace/assets/avatar.jpg`

## 示例

**用户**：帮我挑个头像
**AI**：打开网站让用户挑选，告诉用户挑好了告诉 AI

**用户**：我喜欢那个蓝色头发的
**AI**：（找到对应图片，下载到 workspace/assets/avatar.jpg）

**用户**：这个不错
**AI**：（下载当前展示的图片）

## 注意事项
- 默认保存路径：`workspace/assets/avatar.jpg`
- 支持 PNG、JPG、WebP 格式
