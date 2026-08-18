<?php
date_default_timezone_set('Asia/Taipei');
$server_time = date("Y-m-d H:i:s");
$team_name = "智冷未來";
$school_name = "彰師附工";
?>
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title><?php echo $team_name; ?> - <?php echo $school_name; ?>教室溫度監測</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .box {
            border: 1px solid #ccc;
            padding: 15px;
            max-width: 400px;
        }
        .temp {
            font-size: 48px;
            font-weight: bold;
            margin: 10px 0;
        }
        .alert {
            padding: 10px;
            margin-top: 10px;
            border-radius: 4px;
        }
        .cool { background-color: #d4edda; color: #155724; }
        .warm { background-color: #fff3cd; color: #856404; }
        .hot { background-color: #f8d7da; color: #721c24; }
        .chart {
            margin-top: 15px;
        }
        iframe {
            width: 100%;
            height: 250px;
            border: 1px solid #ddd;
        }
    </style>
</head>
<body>

    <div class="box">
        <h3><?php echo $school_name; ?> 教室溫度監測</h3>       
        <hr>

        <div>即時溫度：</div>
        <div class="temp"><span id="tempValue">--</span> °C</div>

        <div id="alertCard" class="alert warm">資料讀取中...</div>

        <div class="chart">
            <div>溫度歷史圖表：</div>
            <iframe id="3451994" src="https://thingspeak.mathworks.com/channels/3451994/api_keys"></iframe>
        </div>
    </div>

    <script>
        const channelID = "YOUR_CHANNEL_ID"; 
        const readApiKey = "YOUR_READ_API_KEY"; 

        async function updateData() {
            if (channelID === "YOUR_CHANNEL_ID") {
                let mockTemp = (25 + Math.random() * 4).toFixed(1);
                renderTemperature(mockTemp);
                return;
            }

            const url = `https://api.thingspeak.com/channels/${3451994}/feeds/last.json?api_key=${2ZVSF5QJ3A6FLQGU}`;

            try {
                const response = await fetch(url);
                const data = await response.json();
                
                if (data && data.field1) {
                    const temp = parseFloat(data.field1).toFixed(1);
                    renderTemperature(temp);
                }
            } catch (error) {
                console.error("讀取失敗：", error);
            }
        }

        function renderTemperature(temp) {
            document.getElementById('tempValue').innerText = temp;
            const alertCard = document.getElementById('alertCard');

            if (temp < 26) {
                alertCard.className = "alert cool";
                alertCard.innerHTML = "建議開啟電風扇即可，無需開冷氣。";
            } else if (temp >= 26 && temp < 28) {
                alertCard.className = "alert warm";
                alertCard.innerHTML = "冷氣建議設定 27°C + 搭配循環扇。";
            } else {
                alertCard.className = "alert hot";
                alertCard.innerHTML = "室內較熱，請先開窗通風 5 分鐘再開啟冷氣。";
            }
        }

        updateData();
        setInterval(updateData, 15000);
    </script>

</body>
</html>
