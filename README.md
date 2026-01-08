# ACGNnsj.github.io
<script type="module">
    const newWholeHtml =
    `<!DOCTYPE html>
    <html>
    <head>
        <meta charset="UTF-8">
        <style>
            iframe {
                width: 100%;
                border: none;
                min-height: 100px;
            }
        </style>
    </head>
    <body>
    <!-- 嵌入game.html，绑定id方便JS操作 -->
    <iframe id="Silver" src="https://acgnnsj.github.io/Silver-Eyes/" height="1080"></iframe>
    <iframe id="gameIframe" src="https://acgnnsj.github.io/game-of-life/" height="600"></iframe>
    </body>
    </html>`
    const parser = new DOMParser();
    const newDoc = parser.parseFromString(newWholeHtml, 'text/html');
    // 替换整个HTML根节点
    document.documentElement.replaceWith(newDoc.documentElement);
    // 触发页面重渲染
    document.body.style.display = 'block';
</script>
