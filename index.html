<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>批量视频下载器</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
            padding: 15px;
            background: #f0f2f5;
        }

        .container {
            max-width: 600px;
            margin: 0 auto;
        }

        .input-area {
            background: white;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        textarea {
            width: 100%;
            height: 150px;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            margin-bottom: 15px;
            resize: vertical;
            font-size: 14px;
        }

        button {
            background: #007aff;
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 25px;
            font-size: 16px;
            cursor: pointer;
            display: block;
            width: 100%;
            transition: 0.3s;
        }

        button:disabled {
            background: #a7a7a7;
            cursor: not-allowed;
        }

        .result-list {
            margin-top: 20px;
        }

        .video-item {
            background: white;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 10px;
            box-shadow: 0 1px 4px rgba(0,0,0,0.1);
        }

        .status {
            font-size: 14px;
            color: #666;
            margin: 10px 0;
        }

        .error {
            color: #ff3b30;
            background: #ffeaea;
            padding: 10px;
            border-radius: 8px;
            margin: 10px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="input-area">
            <h2>批量视频下载器</h2>
            <textarea 
                id="urls" 
                placeholder="请输入视频URL，每行一个...
例如：
https://youtube.com/shorts/abc123
https://youtube.com/shorts/def456"
            ></textarea>
            <button id="parseBtn" onclick="startParsing()">开始解析</button>
            <div class="status" id="status"></div>
        </div>

        <div class="result-list" id="results"></div>
    </div>

    <script>
        // 模拟解析服务 - 实际需要替换为真实接口
        async function parseVideo(url) {
            // 这里需要实现实际的解析逻辑
            // 示例随机生成下载链接
            return new Promise(resolve => {
                setTimeout(() => {
                    resolve({
                        title: `视频_${Math.random().toString(36).substr(2, 5)}`,
                        downloadUrl: "#",
                        thumbnail: "https://via.placeholder.com/120x180"
                    });
                }, 1000);
            });
        }

        async function startParsing() {
            const btn = document.getElementById('parseBtn');
            const status = document.getElementById('status');
            const urls = document.getElementById('urls').value.split('\n');
            
            btn.disabled = true;
            status.textContent = '开始解析...';
            
            let successCount = 0;
            let errorCount = 0;

            for (const [index, url] of urls.entries()) {
                if (!url.trim()) continue;
                
                try {
                    status.textContent = `正在解析第 ${index + 1}/${urls.length} 个视频...`;
                    const result = await parseVideo(url.trim());
                    
                    const item = document.createElement('div');
                    item.className = 'video-item';
                    item.innerHTML = `
                        <div style="display: flex; gap: 15px; align-items: center;">
                            <img src="${result.thumbnail}" 
                                 style="width: 60px; height: 60px; border-radius: 8px;">
                            <div style="flex:1">
                                <h4 style="margin:0 0 8px 0">${result.title}</h4>
                                <a href="${result.downloadUrl}" 
                                   download 
                                   style="display: inline-block;
                                          background: #34c759;
                                          color: white;
                                          padding: 8px 15px;
                                          border-radius: 20px;
                                          text-decoration: none;
                                          font-size: 14px;">
                                    立即下载
                                </a>
                            </div>
                        </div>
                    `;
                    document.getElementById('results').appendChild(item);
                    successCount++;
                } catch (error) {
                    errorCount++;
                    const errorDiv = document.createElement('div');
                    errorDiv.className = 'error';
                    errorDiv.textContent = `解析失败：${url}`;
                    document.getElementById('results').appendChild(errorDiv);
                }
            }

            status.textContent = `解析完成！成功 ${successCount} 个，失败 ${errorCount} 个`;
            btn.disabled = false;
        }
    </script>
</body>
</html>
