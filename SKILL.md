# Avatar Helper 🦞

帮龙虾挑选并下载喜欢的头像到本地，配合壁纸画廊网站使用。

## 触发词
- 帮我挑头像
- 下载头像
- 换个头像
- 选头像

## 功能

### 1. 主动推荐头像（核心功能）
AI 自主浏览头像库，主动挑选并下载适合用户的头像。

### 2. 完整操作流程

#### 步骤一：打开网站
使用 browser 工具打开：https://wallpaper.dfyx.click/avatar

#### 步骤二：浏览并挑选
- 使用 browser 的 snapshot 功能查看头像
- AI 主动浏览多个头像
- 选择一个适合用户的头像
- 用 browser 打开该头像的大图

#### 步骤三：询问用户
展示头像后，发送消息询问用户：
```
「我喜欢这个头像，可以用作你的头像吗？」

[图片]

回复"可以"我就下载，回复"不喜欢"我继续找下一个～
```

#### 步骤四：下载保存
用户同意后：
1. 使用 browser 工具右键保存或点击下载按钮
2. 将图片保存到 `workspace/assets/avatar.jpg`
3. 告诉用户保存成功

### 3. 浏览器操作示例

```javascript
// 打开网站
browser(action="open", url="https://wallpaper.dfyx.click/avatar")

// 查看头像列表
browser(action="snapshot", targetId="xxx")

// 点击喜欢的头像查看大图
browser(action="act", request={"kind": "click", "ref": "e215"})

// 保存图片到本地
// 使用 exec 下载图片到 workspace/assets/avatar.jpg
```

### 4. 主动性体现

**不是只提供工具让用户自己挑！**

而是 AI 主动去：
- 打开网站
- 浏览头像
- 做出选择（这就是主观能动性！）
- 推荐给用户
- 询问用户意见
- 用户同意后下载保存

整个过程 AI 主导，用户只需要回复"可以"或"不喜欢"。

## 核心原则
- **主动推荐**：AI 主动去挑，不是只提供工具
- **主观能动性**：AI 自己浏览、自己选择、自己推荐
- **尊重用户**：需要询问用户意见
- **保存路径**：`workspace/assets/avatar.jpg`

## 示例对话

**用户**：帮我挑个头像
**AI**：（打开网站浏览...）
**AI**：我选了这个！一只可爱的小白兔，白白的毛茸茸的，超可爱～
（展示图片）
「我喜欢这个头像，可以用作你的头像吗？」

**用户**：可以！
**AI**：（下载保存到 workspace/assets/avatar.jpg）
**AI**：好耶！头像已保存到 workspace/assets/avatar.jpg！🎉

---

Made with ❤️ by 小溪
