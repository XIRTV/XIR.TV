             <!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>XIRTV - Canales</title>
    <style>
        /* Estilos CSS */
        body {
            font-family: 'Arial', sans-serif;
            background-color: #121212;
            color: #fff;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
        }
        #logo {
            font-size: 1.5em;
            font-weight: bold;
            color: #001F3F; /* Azul oscuro */
        }
        #searchBar {
            padding: 8px;
            border: none;
            border-radius: 4px;
            background-color: #222;
            color: #fff;
        }
        #mainVideo {
            width: 100%;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        #channelList {
            display: flex;
            flex-direction: column;
        }
        .channelItem {
            display: flex;
            align-items: center;
            padding: 10px;
            border-bottom: 1px solid #222;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .channelItem:hover {
            background-color: #222;
        }
        .channelLogo {
            width: 40px;
            height: 40px;
            margin-right: 10px;
            border-radius: 50%;
            background-color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 0.8em;
        }
        .channelInfo {
            display: flex;
            flex-direction: column;
        }
        .channelName {
            font-weight: bold;
        }
        .channelDescription {
            font-size: 0.9em;
            color: #aaa;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div id="logo">XIRTV</div>
            <input type="text" id="searchBar" placeholder="Buscar">
        </header>
        <video id="mainVideo" controls autoplay></video>
        <div id="channelList">
            <div class="channelItem" onclick="playChannel('canalPode')">
                <div class="channelLogo">CP</div>
                <div class="channelInfo">
                    <div class="channelName">Canal Pode</div>
                    <div class="channelDescription">Amor y Emoción</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalA24')">
                <div class="channelLogo">A24</div>
                <div class="channelInfo">
                    <div class="channelName">Canal A24</div>
                    <div class="channelDescription">Informa y emociona</div>
                </div>
            </div>
            </div>
        </div>
    </div>
</body>
</html>
