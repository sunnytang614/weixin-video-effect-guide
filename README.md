# 视频号特效创作指南 - GitHub Pages 部署包

## 📦 部署文件清单

### 核心文件
- `index.html` - 主页面（25KB）
- `公众号二维码.png`（27KB）

### 素材文件
- `模特头像素材.zip`（2.5MB）
- `模特半身像素材.zip`（7.9MB）

### 视频文件
- `视频1_基本功能介绍.mp4`（23MB）⚠️ **接近GitHub 25MB限制**
- `视频2_贴纸滤镜类教程.mp4`（13MB）✅ 正常
- `视频3_AI图生图类教程.mp4`（7.9MB）✅ 正常

## 🚀 部署到GitHub Pages

### 步骤1：创建仓库
1. 访问 https://github.com/new
2. 仓库名称：`weixin-video-effect-guide`
3. Public 或 Private 均可
4. 点击 Create repository

### 步骤2：上传文件
1. 点击 "Upload files"
2. 将本目录所有文件拖入上传区域
3. 点击 Commit changes

**⚠️ 注意事项：**
- 视频1（23MB）可能会因为接近25MB限制而上传失败
- 如果视频1上传失败，请尝试：
  1. 继续压缩视频1（目标<20MB）
  2. 或使用Git命令行上传：`git lfs track "*.mp4"`

### 步骤3：启用GitHub Pages
1. 进入仓库 Settings
2. 左侧菜单 → Pages
3. Source 选择：main branch
4. 点击 Save

### 步骤4：访问页面
等待1-2分钟后，访问：
```
https://你的GitHub用户名.github.io/weixin-video-effect-guide/
```

## 📱 微信访问
部署完成后，直接将GitHub Pages链接发送到微信即可打开！

## 🎯 页面功能
- ✅ 深色主题设计，移动端适配
- ✅ 3个视频教程（基本功能、贴纸滤镜、AI图生图）
- ✅ 创作灵感中心（热点报告、特效生成工具、灵感文档）
- ✅ 素材下载（模特头像素材、模特半身像素材）
- ✅ 激励政策说明（流量券、现金激励）
- ✅ 常见问题解答
- ✅ 问题反馈入口

## 🔄 更新日志
- 2025-04-07: 首次发布

## 💡 如果视频1上传失败

### 方案1：继续压缩视频1
推荐使用 HandBrake（免费）：
- 分辨率：960x540（540p）
- 比特率：800kbps
- 帧率：20fps
- 预期大小：约8-10MB

### 方案2：使用Git LFS
```bash
# 在仓库目录执行
git lfs install
git lfs track "*.mp4"
git add .
git commit -m "Add video files with LFS"
git push
```

### 方案3：临时先上线其他2个视频
- 删除视频1文件
- 先上线页面
- 视频1准备好后再更新

## 📞 技术支持
如有问题，请检查：
1. GitHub仓库是否正确
2. Pages是否已启用
3. 等待1-2分钟让页面生效
