# bilicc-json2srt.py

哔哩哔哩 CC 字幕 JSON 转 SRT 格式

## 使用方法

将 json2srt.py 和要转换的 JSON 文件放在同一个文件夹下，然后运行。

转换前：

```
XXdir
  |-- json2srt.py
  |-- foo.json
  '-- bar.json
```

转换后：

```
XXdir
  |-- json2srt.py
  |-- foo.json
  |-- bar.json
  |-- foo.srt
  '-- bar.srt
```

## 哔哩哔哩 JSON 格式

```json
{
  body: [
    {
      content: "CONTENT",
      from: START_SECOND.START_MILLISECOND,
      location: 2,
      to: END_SECOND.END_MILLISECOND
    },
    ...
  ]
}
```
