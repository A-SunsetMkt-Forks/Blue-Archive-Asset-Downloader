# 碧蓝档案素材下载器 / Blue Archive Asset Downloader / ブルアカアッセトダウンローダー

<div align="center">本项目可以从不同服务器下载<!--并读取-->碧蓝档案的素材，现支援中国版、国际版、日本版。</div>

## 主要功能

- **多服务器支持**：可从中国、国际、日本三个版本的服务器下载素材。
- **多线程下载**：支持多线程快速下载。

## 素材内容

下载的文件类型包括：

- Bundle
- Media
- Table

## 环境要求

- Python 3.10 或更高版本

## 先决条件

请确保已安装 Python，并安装必要的库：

```shell
pip install -r requirements.txt
```
## 使用说明
使用下列命令行参数运行 `asset_downloader.py` 脚本（示例）：

```shell
python resource_downloader.py --threads 30 --version 1.8.1 --region cn --downloading-extract True --proxy http://0.0.0.0:0000 --max-retries 10 --search azusa,ハナコ,下江小春,아지타니히후미,聖園彌香
```
## 参数说明

- `--threads`, `-t` 同时下载的线程数。
<!--- `--version`, `-v` 游戏版本号，不填则自动获取。-->
- `--region`, `-g` **`*`**服务器区域：`cn` (中国), `gl` (国际), `jp` (日本)。
- `--raw`, `-r` 指定原始文件输出位置。
- `--extract`, `-e` 指定解压文件输出位置。
- `--temporary`, `-m` 指定临时文件输出位置。
<!-- - `--downloading-extract`, `-d` 是否在下载时解开文件。 -->
- `--proxy`, `-p` 设置HTTP代理。
- `--max-retries`, `-x` 下载时的最大重试次数。
- `--search`, `-s` 指定需要检索并下载的文件的关键词，使用半角英文逗号`,`分隔。
> **`*`** :必选的选项
## TODO

- **流式解包**：下载时解开文件。
- **flatbuf**
- **获取指定版本的资源**
<!-- - **在线预览数据**：WebUI。 -->


## 关于项目
本项目采用 [MIT 许可证](LICENSE)。

部分内容参照自：
- [Blue-Archive---Asset-Downloader](https://github.com/K0lb3/Blue-Archive---Asset-Downloader)。
- [BlueArchiveDownloaderJP](https://github.com/fiseleo/BlueArchiveDownloaderJP)。
- [BA-AD](https://github.com/Deathemonic/BA-AD)。
- [Il2CppDumper](https://github.com/Perfare/Il2CppDumper/tree/master)。

## 免责声明 / Disclaimer
该仓库仅供学习和展示用途，不托管任何实际资源。请注意，所有通过本项目下载的内容均应仅用于合法和正当的目的。开发者不对任何人因使用本项目而可能引发的直接或间接的损失、损害、法律责任或其他后果承担任何责任。用户在使用本项目时需自行承担风险，并确保遵守所有相关法律法规。如果有人使用本项目从事任何未经授权或非法的活动，开发者对此不承担任何责任。用户应对自身的行为负责，并了解使用本项目可能带来的任何风险。
This project is intended solely for educational and demonstrative purposes and does not provide any actual resources. Please note that all content downloaded through this project should only be used for legal and legitimate purposes. The developers are not liable for any direct or indirect loss, damage, legal liability, or other consequences that may arise from the use of this project. Users assume all risks associated with the use of this project and must ensure compliance with all relevant laws and regulations. If anyone uses this project for any unauthorized or illegal activities, the developers bear no responsibility. Users are responsible for their own actions and should understand the risks involved in using this project.
