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
            color: #e50914;
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
            <div id="logo">VeoPlay</div>
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
            <div class="channelItem" onclick="playChannel('canalPakaPaka')">
                <div class="channelLogo">PP</div>
                <div class="channelInfo">
                    <div class="channelName">Canal Paka Paka</div>
                    <div class="channelDescription">Para los más pequeños</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalRetro')">
                <div class="channelLogo">RT</div>
                <div class="channelInfo">
                    <div class="channelName">Canal Retro</div>
                    <div class="channelDescription">Recuerdos inolvidables</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalCronica')">
                <div class="channelLogo">CT</div>
                <div class="channelInfo">
                    <div class="channelName">Crónica TV</div>
                    <div class="channelDescription">Noticias al instante</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canal9Litoral')">
                <div class="channelLogo">C9L</div>
                <div class="channelInfo">
                    <div class="channelName">Canal 9 Litoral</div>
                    <div class="channelDescription">Noticias de la región</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalMagicoRetro')">
                <div class="channelLogo">MR</div>
                <div class="channelInfo">
                    <div class="channelName">Mágico Retro</div>
                    <div class="channelDescription">Recuerdos mágicos</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalInvasivo')">
                <div class="channelLogo">IV</div>
                <div class="channelInfo">
                    <div class="channelName">Invasivo TV</div>
                    <div class="channelDescription">Contenido invasivo</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalCaillou')">
                <div class="channelLogo">CL</div>
                <div class="channelInfo">
                    <div class="channelName">24/7 CAILLOU TV</div>
                    <div class="channelDescription">Caillou todo el día</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalLUZ')">
                <div class="channelLogo">CL</div>
                <div class="channelInfo">
                    <div class="channelName">Canal LUZ</div>
                    <div class="channelDescription">Emisora cristiana</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canal10')">
                <div class="channelLogo">C10</div>
                <div class="channelInfo">
                    <div class="channelName">Canal 10</div>
                    <div class="channelDescription">Noticias y entretenimiento</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canalC5sf')">
                <div class="channelLogo">C5</div>
                <div class="channelInfo">
                    <div class="channelName">Canal C5sf</div>
                    <div class="channelDescription">Información y más</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canal7Neuquen')">
                <div class="channelLogo">C7</div>
                <div class="channelInfo">
                    <div class="channelName">Canal 7 Neuquén</div>
                    <div class="channelDescription">Noticias de Neuquén</div>
                </div>
            </div>
             <div class="channelItem" onclick="playChannel('sonicaArgentina')">
                <div class="channelLogo">SA</div>
                <div class="channelInfo">
                    <div class="channelName">Sonica Argentina</div>
                    <div class="channelDescription">Música y más</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('laPanteraRosa')">
                <div class="channelLogo">PR</div>
                <div class="channelInfo">
                    <div class="channelName">24/7 La Pantera Rosa</div>
                    <div class="channelDescription">Dibujos animados</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('miniTV')">
                <div class="channelLogo">MT</div>
                <div class="channelInfo">
                    <div class="channelName">MINI.TV</div>
                    <div class="channelDescription">Entretenimiento</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('cn247')">
                <div class="channelLogo">CN</div>
                <div class="channelInfo">
                    <div class="channelName">CN 24/7 EN VIVO</div>
                    <div class="channelDescription">Noticias</div>
                </div>
            </div>
             <div class="channelItem" onclick="playChannel('netTV')">
                <div class="channelLogo">NT</div>
                <div class="channelInfo">
                    <div class="channelName">NET TV</div>
                    <div class="channelDescription">Noticias y entretenimiento</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('clanTV')">
                <div class="channelLogo">CT</div>
                <div class="channelInfo">
                    <div class="channelName">CLAN TV</div>
                    <div class="channelDescription">Para los más pequeños</div>
                </div>
            </div>
             <div class="channelItem" onclick="playChannel('canal13')">
                <div class="channelLogo">C13</div>
                <div class="channelInfo">
                    <div class="channelName">CANAL13</div>
                    <div class="channelDescription">Noticias y entretenimiento</div>
                </div>
            </div>
            <div class="channelItem" onclick="playChannel('canal10mdp')">
                <div class="channelLogo">C10</div>
                <div class="channelInfo">
                    <div class="channelName">Canal 10 Mar del Plata En Vivo</div>
                    <div class="channelDescription">Noticias y entretenimiento</div>
                </div>
            </div>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/hls.js@latest"></script>
    <script>
        var video = document.getElementById('mainVideo');
        var hls = new Hls();
        function playChannel(channelId) {
            var videoSource = '';
            // Detach existing HLS stream if any
            if (hls) {
                hls.detachMedia();
                hls.destroy();
                hls = new Hls(); // Re-instantiate hls object
            }
            switch (channelId) {
                case 'canalPode':
                    videoSource = 'URL_DEL_CANAL_PODE.mp4'; // Reemplaza con la URL real
                    break;
                case 'canalA24':
                    videoSource = 'https://g1.vxral-hor.transport.edge-access.net/a15/ngrp:a24-100056_all/a24-100056.m3u8';
                    break;
                case 'canalPakaPaka':
                    videoSource = 'https://joy.nx-pc.edge-apps.net/hls/fmk71-o60f6-lb4p-jbad9.m3u8';
                    break;
                case 'canalRetro':
                    videoSource = 'https://live20.bozztv.com/akamaissh101/ssh101/retrotvcr2025/playlist.m3u8';
                    break;
                case 'canalCronica':
                    videoSource = 'https://g4.mc-hor.transport.edge-access.net/a14/ngrp:cronicatv_video1-100044_all/playlist.m3u8';
                    break;
                case 'canal9Litoral':
                    videoSource = 'https://stream.arcast.live/canal9litoral/ngrp:canal9litoral_all/playlist.m3u8';
                    break;
                case 'canalMagicoRetro':
                    videoSource = 'https://live20.bozztv.com/giatv/giatv-retromagico/retromagico/playlist.m3u8';
                    break;
                case 'canalInvasivo':
                    videoSource = 'https://tv.invasivamedia.com/hls/limtv.m3u8';
                    break;
                case 'canalCaillou':
                    videoSource = 'https://d2zq3jgz2yetok.cloudfront.net/v1/master/3722c60a815c199d9c0ef36c5b73da68a62b09d1/cc-71a686zhs51em/master.m3u8';
                    break;
                case 'canalLUZ':
                    videoSource = 'https://g1.mc-hor.transport.edge-access.net/a11/ngrp:canal_luz01-100009_all/Playlist.m3u8?sense=true';
                    break;
                 case 'canal10':
                    videoSource = 'https://g3.mc-hor.transport.edge-access.net/a10/ngrp:canal10junin-100056_all/Playlist.m3u8?sense=true';
                    break;
                 case 'canalC5sf':
                    videoSource = 'https://stream.arcast.com.ar/c5sf/c5sf/chunklist_w82661505.m3u8';
                    break;
                case 'canal7Neuquen':
                    videoSource = 'https://stream.arcast.com.ar/c7nq/ngrp:c7nq_all/playlist.m3u8';
                    break;
                case 'sonicaArgentina':
                    videoSource = 'https://tv.streamcasthd.com:3076/live/sonicaargentinalive.m3u8';
                    break;
                case 'laPanteraRosa':
                    videoSource = 'https://linear-1069.frequency.stream/mt/plex/1069/hls/master/playlist_1920x1080.m3u8';
                    break;
                case 'miniTV':
                    videoSource = 'https://live20.bozztv.com/akamaissh101/ssh101/monitvhd/playlist.m3u8';
                    break;
                case 'cn247':
                    videoSource = 'https://panel.host-live.com:19360/cn247tv/cn247tv.m3u8';
                    break;
                case 'netTV':
                    videoSource = 'https://unlimited1-us.dps.live/nettv/nettv.smil/playlist.m3u8';
                    break;
                case 'clanTV':
                    videoSource = 'https://rtvelivestream-rtveplayplus.rtve.es/rtvesec/int/clan_int_main_dvr_720.m3u8';
                    break;
               case 'canal13':
                    videoSource = 'https://jireh-1-hls-video-br-isp.dps.live/hls-video/10b92cafdf3646cbc1e727f3dc76863621a327fd/t13/t13.smil/playlist.m3u8?auth-token=&dpssid=b268736546468d9b54c46e';
                    break;
               case 'canal10mdp':
                    videoSource = 'https://g5.mc-hor.transport.edge-access.net/a12/ngrp:canal10mdq-100044_all/Playlist.m3u8?sense=true';
                    break;
                default:
                    videoSource = '';
            }
            // Utiliza HLS.js si es compatible
            if (Hls.isSupported()) {
                hls.loadSource(videoSource);
                hls.attachMedia(video);
                hls.on(Hls.Events.MANIFEST_PARSED, function() {
                    video.play();
                });
            }
            // Si HLS no es compatible, intenta reproducir el video directamente
             else if (video.canPlayType('application/vnd.apple.mpegurl')) {
                video.src = videoSource;
                video.addEventListener('loadedmetadata', function() {
                    video.play();
                });
            }
            else {
                console.log('HLS is not supported on this browser.');
            }
        }
    </script>
</body>
</html>
