# OBS NMS FLV

## 技术方案

- 使用 `OBS` 进行推流
- 使用 `node-media-server` 作为服务器
- 使用 `flv.js` 进行拉流

## 启动

1. 打开 `OBS`，设定直播服务器为 `rtmp://localhost:1935/live`，推流码为 `STREAM_NAME`

2. 启动 `node-media-server`

```bash
node nms.js
```

3. 启动 `express` 并访问 `http://localhost:3000/flv.html`

视频流地址为：`http://localhost:8000/live/STREAM_NAME.flv`
