# Bilibili 用户精确数据爬虫

个人科研用的，用来快速判断一个用户视频创作者还是消费者，即有没有投稿过视频。

一个爬取b站用户信息的Python爬虫。

#### **亮点**：能爬取到**精确数量**的阅读数、播放数、获赞数、粉丝量
不会是获赞数4579.7万，而是获赞数45796729

#### 好用的话记得给个star

## 运行环境和依赖

* Python 3.6 或更高版本
* Selenium 库
* OpenPyXL 库
* WebDriverManager 库

安装依赖：
pip install selenium openpyxl webdriver_manager

## 功能
此爬虫可以获取以下用户信息：

* 昵称
* 个人简介
* 关注数
* 粉丝数
* 获赞数
* 播放数
* 阅读数
* 视频投稿数

这些数据将保存在名为 output.xlsx 的 Excel 文件中。

## 使用方法
* 将用户ID保存到名为 user_ids.txt 的文件中，每行一个。
* 运行 Python 爬虫脚本：python bilibili_user_info_scraper.py（或pycharm等软件打开运行）。
* 当提示登录时，请手动登录您的 Bilibili 账户。登录完成后，按回车键继续。
* 爬虫将开始抓取用户信息，并将结果保存到 output.xlsx 文件中。
* 完成后，关闭浏览器并检查 output.xlsx 文件以查看提取的数据。

## 注意事项
1. 请确保您已经安装了所有必要的依赖库。
2. 确保您已经安装了 Google Chrome 浏览器，因为此爬虫使用 Chrome WebDriver。
3. 如果您遇到任何问题，请检查用户ID是否正确，并确保您的网络连接正常。
4. 在输出结果中，如果某个单元格的值为 -1，表示该值未能成功抓取。
