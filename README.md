# 🎬 Bilingual Video Marketing Page
# 双语视频营销网页

Create an AI promotional video, write Chinese–English marketing copy, and publish your own video webpage.

制作 AI 宣传视频，撰写中英双语营销文案，并发布自己的视频网页。

---

## 🎯 Learning Objectives / 学习目标

By completing this project, you will learn to:

完成本项目后，你将能够：

- Plan a promotional video for a specific audience.  
  为特定目标受众策划宣传视频。
- Use an AI video tool to create visual content.  
  使用 AI 视频工具制作视觉内容。
- Write persuasive Chinese and English marketing copy.  
  撰写有说服力的中英文营销文案。
- Edit a simple JavaScript configuration.  
  修改简单的 JavaScript 配置。
- Publish and test a webpage using GitHub Pages.  
  使用 GitHub Pages 发布并测试网页。

## 🧰 What You Need / 所需工具

- Access to an AI video-generation tool available for your class  
  可供课堂使用的 AI 视频生成工具
- A GitHub account  
  GitHub 账号
- A text editor or GitHub’s file editor  
  文本编辑器或 GitHub 文件编辑器
- A modern web browser  
  现代网页浏览器

No backend server or API key is needed for this webpage.

本网页不需要后端服务器或 API 密钥。

---

## Part 1 — Create Your Video / 制作视频

### 1. Choose your campaign / 选择营销主题

Choose a fictional product, service, or event.

选择一个虚构的产品、服务或活动。

Examples / 示例：

- A student-friendly café / 面向学生的咖啡馆
- A reusable water bottle / 可重复使用的水瓶
- A campus cultural festival / 校园文化节

Before generating your video, answer:

生成视频前，请回答：

1. Who is your target audience? / 你的目标受众是谁？
2. What is your main message? / 你的核心信息是什么？
3. What should viewers do next? / 你希望观众接下来做什么？

### 2. Generate the video / 生成视频

Use the AI video tool demonstrated by your instructor.
Tool access and generation limits may vary.

使用教师演示的 AI 视频工具。
工具访问权限及生成额度可能有所不同。

**Example prompt / 提示词示例：**

> Create a short promotional video for a fictional café called
> Morning Light. Show coffee being poured, warm sunlight, and a
> welcoming interior. Use gentle camera movement and a calm,
> friendly mood. The target audience is university students
> looking for somewhere to relax. Do not include on-screen text;
> we will add bilingual marketing copy on the webpage.

For this beginner project, aim for a short video without spoken dialogue.

本入门项目建议制作不含人物对白的短视频。

Review the output, download your video, and name it:

检查生成结果，下载视频，并将文件命名为：

```text
promo.mp4
```

Use an MP4 suitable for browser playback. Renaming a file to `.mp4`
does not convert its actual format.

请使用适合浏览器播放的 MP4 视频。仅将文件扩展名改为 `.mp4`
并不会转换其实际格式。

### 3. Write bilingual copy / 撰写双语文案

Prepare four pieces of text:

准备以下四项内容：

| Field / 字段 | Example / 示例 |
|---|---|
| English heading / 英文标题 | Your daily moment of calm |
| Chinese heading / 中文标题 | 给忙碌的你，一杯慢下来的时光 |
| English subheading / 英文副标题 | Fresh coffee. Warm spaces. Make yourself at home. |
| Chinese subheading / 中文副标题 | 一杯现磨咖啡，一个温暖角落，让每一天从容开始。 |

**Adapt the message for each audience rather than translating word for word.**

**根据不同语言受众调整表达，而不是逐字翻译。**

---

## Part 2 — Build Your Page / 制作网页

### 1. Organize your files / 整理文件

Keep these files in the repository’s top-level folder:

将以下文件放在仓库根目录：

```text
bilingual-video/
├── README.md
├── index.html
├── script.js
└── promo.mp4
```

| File / 文件 | Purpose / 用途 |
|---|---|
| `README.md` | Project instructions / 项目说明 |
| `index.html` | Page structure and styling / 网页结构与样式 |
| `script.js` | Default content and preview behavior / 默认内容与预览功能 |
| `promo.mp4` | Your promotional video / 宣传视频 |

### 2. Edit your published content / 修改发布内容

Open `script.js` and find the `defaults` object.

打开 `script.js`，找到 `defaults` 对象。

Replace the example values with your own content:

将示例内容替换为你的文案和视频路径：

```javascript
const defaults = {
  videoUrl: "promo.mp4",
  titleEn: "Your daily moment of calm",
  titleZh: "给忙碌的你，一杯慢下来的时光",
  subtitleEn: "Fresh coffee. Warm spaces. Make yourself at home.",
  subtitleZh: "一杯现磨咖啡，一个温暖角落，让每一天从容开始。"
};
```

Keep the property names, quotation marks, commas, and braces intact.

请保留属性名称、引号、逗号和大括号。

If your text needs double quotation marks, escape them:

如果文案中需要使用英文双引号，请进行转义：

```javascript
titleEn: "Find your \"me time\""
```

### 3. Preview the page / 预览网页

Open `index.html` in your browser.

在浏览器中打开 `index.html`。

Use the editor to:

使用编辑器：

1. Enter a video URL or file path. / 输入视频网址或文件路径。
2. Edit both language versions. / 修改两种语言的文案。
3. Click **Update preview / 更新预览**.
4. Check the text and play the video. / 检查文案并播放视频。

> **Important:** Form edits only change the current preview.
> They are not saved to GitHub and disappear when you reload.
> To publish changes, update `defaults` in `script.js` and commit the file.
>
> **重要：** 表单修改仅影响当前预览，不会保存到 GitHub，
> 刷新后也不会保留。若要发布修改，请更新 `script.js`
> 中的 `defaults`，并提交文件。

### Video paths / 视频路径

For a video beside `index.html`, use:

视频与 `index.html` 位于同一目录时：

```text
promo.mp4
```

For a video inside a `videos` folder, use:

视频位于 `videos` 文件夹内时：

```text
videos/promo.mp4
```

You may also use a publicly accessible direct video URL.

也可以使用可公开访问的视频文件直链。

A YouTube watch page, GitHub file-view page, or private sharing page
is not a direct video file URL.

YouTube 观看页面、GitHub 文件浏览页面或私人分享页面，
都不是视频文件直链。

---

## 🚀 Publish / 发布

1. Create a public GitHub repository.  
   创建公开的 GitHub 仓库。

2. Upload your project files. Keep the video small enough for
   GitHub’s upload limits.  
   上传项目文件，确保视频大小符合 GitHub 上传限制。

3. Open **Settings → Pages**.  
   打开 **Settings → Pages**。

4. Choose **Deploy from a branch** as the publishing source.  
   选择 **Deploy from a branch** 作为发布来源。

5. Select the branch containing your files, usually `main`,
   and the `/(root)` folder. Save.  
   选择存放文件的分支，通常为 `main`，以及 `/(root)` 目录，然后保存。

6. Wait for deployment and open the site address shown by GitHub.  
   等待部署完成，打开 GitHub 显示的网站地址。

A project site address usually looks like:

项目网站地址通常如下：

```text
https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/
```

Test the published page on both a computer and a phone.

请在电脑和手机上测试发布后的网页。

---

## 🔧 Troubleshooting / 常见问题

| Problem / 问题 | What to check / 检查方法 |
|---|---|
| Video does not load / 视频无法加载 | Check the path, filename capitalization, format, and access permissions. / 检查路径、文件名大小写、格式和访问权限。 |
| Upload fails / 上传失败 | Reduce the video file size and check GitHub’s upload limits. / 压缩视频并检查 GitHub 上传限制。 |
| Preview edits disappear / 预览修改消失 | Save final content in `script.js`, not only in the form. / 将最终内容保存到 `script.js`，不要只修改表单。 |
| Old content still appears / 仍显示旧内容 | Confirm the commit and deployment succeeded, then refresh. / 确认提交与部署成功后刷新网页。 |
| JavaScript stops working / JavaScript 无法运行 | Check quotation marks, commas, braces, and the browser console. / 检查引号、逗号、大括号及浏览器控制台。 |
| Published page is missing / 发布后找不到网页 | Confirm `index.html` is in the selected publishing folder. / 确认 `index.html` 位于所选发布目录。 |

---

## ✅ Submission Checklist / 提交清单

- [ ] A promotional video that matches the target audience  
      符合目标受众的宣传视频
- [ ] An English heading and subheading  
      英文标题和副标题
- [ ] A Chinese heading and subheading  
      中文标题和副标题
- [ ] Final content saved in `script.js`  
      最终内容已保存至 `script.js`
- [ ] A working GitHub Pages site  
      可正常访问的 GitHub Pages 网站
- [ ] Repository address and published website address  
      仓库地址和已发布的网站地址
- [ ] A short reflection explaining your marketing choices  
      简短反思，说明你的营销选择

### Reflection questions / 反思问题

1. How does your video appeal to your target audience?  
   你的视频如何吸引目标受众？

2. What did you change between the Chinese and English versions, and why?  
   中英文版本之间做了哪些调整？为什么？

3. Which version is more persuasive? What feedback supports your view?  
   哪个版本更有说服力？有哪些反馈支持你的判断？

4. What would you improve after testing the page?  
   测试网页后，你会做哪些改进？

## 📊 Suggested Assessment / 建议评分标准

| Component / 项目 | Weight / 比例 |
|---|---:|
| Target audience and marketing message / 目标受众与营销信息 | 25% |
| Quality of bilingual copy / 双语文案质量 | 30% |
| Video relevance and quality / 视频相关性与质量 | 25% |
| Working webpage and explanation of changes / 网页功能与修改说明 | 20% |

---

## 🤝 Responsible Creation / 负责任的创作

- Use content you created or have permission to use.  
  使用原创内容或已获得使用许可的素材。
- Avoid misleading product claims and fabricated testimonials.  
  避免误导性产品宣传和虚构用户评价。
- Label the video as an AI-generated class project.  
  标明视频为 AI 生成的课堂作品。
- Do not upload passwords, API keys, or private information.  
  不要上传密码、API 密钥或私人信息。
- If you include speech, add accurate captions as an extension task.  
  如视频包含对白，请将准确字幕作为拓展任务。

## ⭐ Optional Extensions / 拓展任务

- Add a bilingual call-to-action button. / 添加双语行动按钮。
- Add a Chinese–English language switch. / 添加中英文切换功能。
- Make a second copy version for peer comparison. / 制作第二版文案供同学比较。
- Create a visitor-facing page without the editor form. / 制作不含编辑表单的访客页面。
- Add captions for spoken content. / 为有声内容添加字幕。
