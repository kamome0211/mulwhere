<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Open Website Permanently</title>
</head>
<body>
    <button onclick="openWebsitePermanently()">Open Website Permanently</button>

    <script>
        function openWebsitePermanently() {
            setInterval(function() {
                // 新しいウィンドウを開く
                const newWindow = window.open('chrome-extension://jbddgjglgkkneonnineaohdhabjbgopi/pages/message-page.html?mode=blocked&category=302', '_blank', 'width=600,height=400');

                // ウィンドウが閉じられた場合、再度新しいウィンドウを開く
                newWindow.addEventListener('beforeunload', function() {
                    openWebsitePermanently();
                });
            }, 0); // 1秒ごとに新しいウィンドウを開く（ポップアップブロッカーを避けるための遅延）
        }
    </script>
</body>
</html>


