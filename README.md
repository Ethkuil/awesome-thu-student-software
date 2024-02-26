# awesome-thu-student-software
本项目收录主要由清华大学在校学生开发/维护的实用 **开源** 软件。目前收录的软件都聚焦于校园生活。

要求：
* 实用、可用。具有重要纪念/参考意义的可破例，如T大树洞。
* 「仅供学习参考、不应传播」的软件一般不收录，如文泉学堂PDF下载。

若有软件已失效，如果您愿意在 Issue / PR 中提醒的话，不胜感激！

> 文档模板、学习资源 等各种杂项「资源」，[THU Services](https://thu.services) 汇总得很好。实际上其中也有对软件工具的汇总，但有点需要二次淘金（如其中查洗衣机状态的多个工具都没有THUInfo好用）。

## 项目

| 项目名 | 简介 | 适用平台 & 开发语言 |
|-|-|-|
| [thu-learn-lib](https://github.com/Harry-Chen/thu-learn-lib) | 提供网络学堂2018的接口。</br>[thu-learn-lib 开发小记](https://harrychen.xyz/2019/02/09/thu-learn-lib/)| JavaScript库。</br>使用 TypeScript 开发。|
| [thu-info-lib](https://github.com/thu-info-community/thu-info-app/tree/HEAD/packages/thu-info-lib) | 提供信息门户的接口。 | JavaScript库。</br>使用 TypeScript 开发。|
| [THUInfo](https://github.com/thu-info-community/thu-info-app) | 集成各种校园信息。如GPA、图书馆资源、教室资源、洗衣机、学生卡消费、新闻、课表…… | 支持 Android、iOS。</br>使用 Typescript、React Native 开发。|
| [Learn Helper](https://github.com/Harry-Chen/Learn-Helper) | 清华大学网络学堂浏览器扩展。便于管理相关信息；可在扩展的图标上看到待处理事项的数量。</br>[Learn Helper 4.0.0 开发感想](https://harrychen.xyz/2019/02/22/learn-helper-v4/)| 使用 Typescript、React 开发。|
| [learnX](https://github.com/robertying/learnX) | 清华大学网络学堂 App。| 支持 Android、iOS、macOS。</br>可联动 [课程信息共享计划](https://tsinghua.app/courses)（共享课程的上课时间地点）。</br>使用 Typescript、React Native 开发。|
| [T大树洞](https://github.com/treehollow/) | 旧洞。后由于某些原因主动关停。目前可使用 [新T树洞](https://new-t.github.io/)。| [后端](https://github.com/treehollow/treehollow-backend)使用 Go 开发。</br>[网页版前端](https://github.com/treehollow/webhole)使用 React, [iOS/macOS版](https://github.com/treehollow/treehollow-v3-ios)使用 SwiftUI，[Android版](https://github.com/treehollow/treehollow-v3-android)主要使用 Kotlin。 |
| [新T树洞](https://git.thu.monster/newthuhole/) | [树洞网址](https://new-t.github.io/) | [后端](https://git.thu.monster/newthuhole/hole-backend-rust)使用 Rust 开发。</br>[网页版前端](https://git.thu.monster/newthuhole/hole_thu_frontend)使用 React 开发。|

## 小工具、小脚本

[thulearn2018](https://github.com/euxcet/thulearn2018)：网络学堂 CLI，支持在终端中下载课件&作业、查看ddl、提交作业！课件&作业支持自动下载。

例：提交作业从「打开浏览器操作半分钟再在对话框里找文件」->「在当前目录启动终端 `learn submit <file>` 不到10秒」。

  > Windows 下可使用 start 命令以默认应用打开文件：
  > ```powershell
  > start hw1.pdf
  > start hw1.docx
  > ```
  > OS X 和 Linux 中亦有相应的 `open` 和 `xdg-open` 命令。
  > 另外，结合 VS Code/Vim/Emacs 使用本工具也是很好的选择，写作业、交作业一站式完成。VS Code 可安装 [Office Viewer](https://github.com/cweijan/vscode-office) 扩展来预览 word, excel 等文件，可通过 `code` 命令从终端打开文件/目录。
  > ```bash 
  > code <file/directory> # 在当前工作区中打开文件，或将目录打开为新的文件夹
  > code -r <directory>   # 使用新的文件夹替换当前工作区

### 优化网站体验的浏览器脚本

选课：
- [清华选课时间冲突标记器](https://greasyfork.org/zh-CN/scripts/408340-tsinghuacourseconflictmarker)：在选课系统中，检测已选课程，自动将候选课中有冲突时间的课标红。
- [Colorful Course](https://greasyfork.org/en/scripts/456440-colorful-course)：为课程的各志愿报名人数上色，方便确定选课志愿。「必能选上」为绿色，「需抽签」为黄色，「不可能选上」为红色。

> 注：以上两个脚本的 `@match` 写得不太完善，现在会匹配不上选课系统的 URL，需自行修改。已给 `清华选课时间冲突标记器` 提交了修复的 [PR](https://github.com/thuservices/thuservices/pull/54)

网络学堂：
- [网络学堂挂机免重登](https://greasyfork.org/zh-CN/scripts/444728-清华大学网络学堂挂机免重登)：网络学堂后台挂着也不会被让重登了。
- [网络学堂3202助手](https://greasyfork.org/zh-CN/scripts/422447-网络学堂3202助手)：直观展现死线情况，点击即可跳转；导出所有课程至日历；一键标记公告已读；批量保存新课件。

雨课堂：
- [Tsinghua Yukuotang Autoplay](https://greasyfork.org/zh-CN/scripts/422349-tsinghua-yukuotang-autoplay)：一个 JS 脚本实操练习项目，功能为自动播放雨阔糖的视频。

信息门户：
- [清华大学GPA查询](https://greasyfork.org/zh-CN/scripts/420540-清华大学gpa查询)：在信息门户的「全部成绩」页面，计算出每个学期和总的必限、必限任GPA。支持 WebVPN。

  > 若使用手机，则更推荐通过 THUInfo 查询成绩。

### 下载器

改进网络学堂体验的多功能工具基本都有批量下载的功能。

[清华教参服务平台下载器](https://github.com/libthu/reserves-lib-tsinghua-downloader)：从[清华教参服务平台](http://reserves.lib.tsinghua.edu.cn/)下载书籍。自动下载书籍每一页的原图，生成 PDF。免登录。

[清华云盘批量下载器](https://github.com/HuXiao-THU/Tsinghua-Tools)：批量下载给定分享链接下的所有内容，无需逐一点击，避免`size too large`。

[清华云盘仓库和清华邮箱下载](https://github.com/Xiang-cd/THU-downloader)：一个支持UI界面的**清华云盘**个人仓库批量下载, 链接批量下载，**清华邮箱**邮件批量下载工具，为毕业生批量迁移清华云盘内容和备份邮箱提供便利。

## Contributing

欢迎发 [Issue](https://github.com/Ethkuil/awesome-thu-student-software/issues/new) 与 PR。

## License

[MIT](./LICENSE)
