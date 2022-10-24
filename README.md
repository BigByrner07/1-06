
<html lang="en">
  
<head>
  <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="manifest" href="/site.webmanifest">
    <style>
        body {
            background: rgb(140, 214, 30);
        }
          
        [data-tab-info] {
            display: none;
        }
          
        .active[data-tab-info] {
            display: block;
        }
          
        .tab-content {
            font-size: 30px;
            font-family: sans-serif;
            font-weight: bold;
            color: rgb(82, 75, 75);
        }
          
        .tabs {
            font-size: 40px;
            color: rgb(255, 255, 255);
            display: flex;
            margin: 0;
        }
          
        .tabs span {
            background: rgb(28, 145, 38);
            padding: 10px;
            border: 1px solid rgb(255, 255, 255);
        }
          
        .tabs span:hover {
            background: rgb(29, 185, 112);
            cursor: pointer;
            color: black;
        }
    </style>
</head>
  
<body>
    <div class="tabs">
        <span data-tab-value="#tab_1">Deji -1</span>
        <span data-tab-value="#tab_2">Deji -2</span>
        <span data-tab-value="#tab_3">Deji -3</span>
    </div>
  
    <div class="tab-content">
        <div class="tabs__tab active" id="tab_1" data-tab-info>
            <p>
              Deji was born in London and lived there for most his life, but he now lives in Peterborough with his parents. Deji started out posting gaming videos to YouTube, including FIFA. He also used to make short sketches, utilizing a "parody" style in making these sketches, with his brother and dad, but by 2016 he stopped uploding these kinds of videos. Deji has created and still does create a lot of "challenge" and "prank" videos and started releasing music videos in 2017. Deji acquired a lot of his fame by virtue of being in his brother KSI's videos.k.</p>
  
        </div>
        <div class="tabs__tab" id="tab_2" data-tab-info>
            <p>Deji is really cool.</p>
  
        </div>
        <div class="tabs__tab" id="tab_3" data-tab-info>
            <p>deji lives in londonf.</p>
  
        </div>
    </div>
    <script type="text/javascript">
        const tabs = document.querySelectorAll('[data-tab-value]')
        const tabInfos = document.querySelectorAll('[data-tab-info]')
  
        tabs.forEach(tab => {
            tab.addEventListener('click', () => {
                const target = document
                    .querySelector(tab.dataset.tabValue);
  
                tabInfos.forEach(tabInfo => {
                    tabInfo.classList.remove('active')
                })
                target.classList.add('active');
            })
        })
    </script>
</body>
  
</html>
