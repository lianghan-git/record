# 录音播放器

一个简洁美观的静态网页音频播放器，用于播放录音文件。

## 使用方法

### 方法一：手动添加音频文件列表（推荐）

1. 打开 `index.html` 文件
2. 找到 `audioFiles` 数组（大约在第 85 行）
3. 添加您的音频文件名，例如：

```javascript
const audioFiles = [
    '我的录音1.mp3',
    '我的录音2.wav',
    '会议记录.m4a',
];
```

4. 将您的音频文件放在与 `index.html` 相同的文件夹中
5. 保存文件并刷新浏览器

### 方法二：直接在 HTML 中添加音频元素

如果您熟悉 HTML，也可以直接在 `index.html` 的 `<div id="audioContainer">` 部分添加音频元素：

```html
<div class="audio-item">
    <div class="audio-title">录音标题</div>
    <audio controls>
        <source src="您的音频文件.mp3" type="audio/mpeg">
    </audio>
</div>
```

## 支持的音频格式

- MP3 (.mp3)
- WAV (.wav)
- OGG (.ogg)
- M4A (.m4a)
- AAC (.aac)
- FLAC (.flac)
- WebM (.webm)

## GitHub Pages 部署

1. 将整个文件夹上传到 GitHub 仓库
2. 在仓库设置中启用 GitHub Pages
3. 选择主分支（通常是 `main` 或 `master`）
4. 访问 `https://您的用户名.github.io/仓库名/` 即可查看网页

## 注意事项

- 确保音频文件名与代码中的文件名完全匹配（包括大小写）
- 音频文件需要与 `index.html` 在同一目录下
- 如果使用 GitHub Pages，确保音频文件也一并上传到仓库

