# WinRAR_compress_multiple_folders<br>
WinRAR指定参数压缩Python脚本【复数文件夹版】<br>


  
功能：批量压缩拖入的多个文件夹，支持分卷、加密、删除源文件等功能<br>
适用场景：无需筛选层级，直接压缩多个拖入的文件夹内容<br>
注意：需提前安装WinRAR，且脚本仅支持Windows系统<br>
<br>
<br>
python环境安装<br>
www.python.org/downloads/windows/<br>

<br>
    "add": "a",                  # 核心指令：添加文件到压缩包<br>
    "recursive": "-r",           # 递归处理子目录<br>
    "delete_source": "-df",      # 压缩完成后删除源文件，<br>
    "recovery_record": "-rr10",  # 添加10%恢复记录，<br>
    "compress_level": "-m3",     # 压缩级别，None=默认<br>
    "dict_size": "-md32m",       # 字典大小，None=不指定<br>
    "encrypt_filename": "-hp",   # 加密压缩包内文件名，None=不加密文件名<br>
    "exclude_base_path": "-ep1", # 排除压缩包内的基本路径，None=保留完整路径<br>
    "progress_percent": "-idp",   # 显示压缩进度百分比，None=不显示<br>
    "progress_detail": "-idv",    # 显示详细的压缩进度信息，None=不显示<br>
<br>

延迟重试配置（文件系统刷新延迟）<br>
RETRY_MAX = 0       # 最大重试次数（0=不重试）<br>
RETRY_DELAY = 1.0   # 重试间隔时间（秒）<br>

分页显示待压缩文件夹列表时的单页数量<br>
PAGE_SIZE = 100<br>
