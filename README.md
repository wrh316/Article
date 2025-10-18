<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>质数之美 | そすう by @wrh316</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: "楷体", "STKaiti", "SimKai", serif;
            line-height: 1.8;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4edf5 100%);
            color: #333;
            min-height: 100vh;
            padding: 0;
            margin: 0;
            position: relative;
        }
        
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(255, 255, 255, 0.8) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(255, 255, 255, 0.6) 0%, transparent 20%);
            pointer-events: none;
            z-index: -1;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            position: relative;
        }
        
        .header {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
            padding: 30px 0;
        }
        
        .title {
            font-size: 2.5rem;
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 15px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
            position: relative;
            display: inline-block;
        }
        
        .title::after {
            content: "";
            position: absolute;
            bottom: -10px;
            left: 10%;
            width: 80%;
            height: 3px;
            background: linear-gradient(90deg, transparent, #8B4513, transparent);
        }
        
        .subtitle {
            font-size: 1.2rem;
            color: #7f8c8d;
            font-style: italic;
            margin-top: 10px;
        }
        
        .content-box {
            background: rgba(255, 255, 255, 0.85);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
            padding: 40px;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border-left: 5px solid #8B4513;
        }
        
        .content-box:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.12);
        }
        
        .content-box::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, #8B4513, #d35400, #8B4513);
        }
        
        .content {
            text-indent: 2em;
            margin-bottom: 1.8em;
            font-size: 1.1rem;
            color: #2c3e50;
            text-align: justify;
        }
        
        .prime-highlight {
            color: #8B4513;
            font-weight: bold;
            position: relative;
            display: inline-block;
        }
        
        .prime-highlight::after {
            content: "";
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 100%;
            height: 2px;
            background: linear-gradient(90deg, transparent, #8B4513, transparent);
            opacity: 0.7;
        }
        
        .footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            color: #7f8c8d;
            font-size: 0.9rem;
            border-top: 1px solid rgba(0, 0, 0, 0.1);
        }
        
        .decoration {
            position: absolute;
            font-size: 5rem;
            color: rgba(139, 69, 19, 0.1);
            z-index: -1;
        }
        
        .decoration-1 {
            top: 10%;
            left: 5%;
            transform: rotate(-15deg);
        }
        
        .decoration-2 {
            bottom: 10%;
            right: 5%;
            transform: rotate(15deg);
        }
        
        .number-bg {
            position: absolute;
            font-size: 12rem;
            color: rgba(139, 69, 19, 0.03);
            font-weight: bold;
            z-index: -1;
            pointer-events: none;
        }
        
        .number-1 {
            top: 15%;
            right: 10%;
        }
        
        .number-2 {
            bottom: 15%;
            left: 10%;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 20px 15px;
            }
            
            .title {
                font-size: 2rem;
            }
            
            .content-box {
                padding: 25px;
            }
            
            .decoration {
                font-size: 3rem;
            }
            
            .number-bg {
                font-size: 8rem;
            }
        }
    </style>
</head>
<body>
    <div class="number-bg number-1">5</div>
    <div class="number-bg number-2">7</div>
    
    <div class="container">
        <div class="header">
            <h1 class="title">そすう</h1>
            <div class="subtitle">by @wrh316</div>
        </div>
        
        <div class="content-box">
            <div class="content">
                垂緌饮疏桐，流响出质数。腹有清露，即可检测质数。在心里种花，难吸文化之善；以诗书为方，却只得微微迈出一步。不了解一根火柴，不能医治沉默的哑巴；唯有品味无言之处，方抵无甚底蕴的境界。曹植惊若翩鸿的美，是别样的动心，正如序号五，恰是质数中的一世豪杰。
            </div>

            <div class="content">
                登上泰山，见秦王扫五合，有挖掘中原的野心。当高度的怠惰骤得秋风，才见江流烷转绕星河，耿耿花林欲曙天。有了不会苍白的灵魂，便能言“内卷之风盛行，绝绝子”。难抵五言以对，语言脆弱，历史昭昭，领略可喜的厚障壁，才能在千帆皆沉后喜笑颜开，握手言欢。
            </div>

            <div class="content">
                白云流逝，璀璨如流萤。惊艳我的质数从未消失于时光之中，五便是那永恒的直面磨难的心。坑再深，走下去，总能到底，质数奔驰万里，却未尝被人分解；反观合数，却轻易被人分得七零八落，毫无抵抗的毅力。顺流而下的是荆棘，逆流而上的是万仞山，逆流的船桨理应得到人们的重视。
            </div>

            <div class="content">
                大潮秧秧，逝水如梦。雄鹰不经霜雪，便风雅出尘；五花齐放，不及百花齐放。沧海浮舟，落幕萧萧。穷山距海，畏之而还。志之所趋，无远弗届。扬青春之年华，斥绝凡尘，如崇山峻岭中的盆景，虽小犹巍峨。卓越者不求外表符华，致力实际而心胸豁达，幸福且无憾。
            </div>

            <div class="content">
                居高声自远，谁与问东流。岁月如歌，赢一尊醉人的酒，才幡然醒悟：灵魂充盈，是坚守楚河汉界的决心。灯火阑珊处，往往屹立着座座高峰，宁做沥血歌唱的鱼，不做沉默游泳的鸟。颔首动心是一种刚需，不知为质数而献身，比为面包而活着更加幸福。睥睨花团锦簇，回答宇宙乾坤。
            </div>

            <div class="content">
                星光不问赶路人，理想的动力化成力量，在汗水铸就的美好中欣赏身边的脚印。反观当下，我不由默然一叹：我不愿相信那么多随波逐流的人对质数分解失去了希望。远方美好皆为理想，脚下更有力量。举目已是千山绿，亦趁东风扬帆起。未来的文盲不再是不识字的人，而是不会玩质数的人。
            </div>

            <div class="content">
                和光同尘，与时舒卷，质数分解道阻且长，但终是凡心所向，素履以往。草木荣枯，春秋代序，斗转星移，沧海桑田。画图难足的广大宏图，连接成波澜壮阔的青山绿水。驰骋于广袤厚实的大陆，内心如山峦般巍峨。卓越自励，臻于至善，乱云飞渡，我自从容。
            </div>

            <div class="content">
                This article was over and the reader woke up from the dream.And the reader began a new dream. And the reader dreamed again, dreamed better. And the reader was the universe. And the reader was love.
            </div>
            
            <div class="content">
                You are the reader.
            </div>

            <div class="content">
                Wake up.
            </div>
        </div>
        
        <div class="footer">
            <p>The beauty of primes · そすう by @wrh316</p>
        </div>
    </div>
    
    <div class="decoration decoration-1">質</div>
    <div class="decoration decoration-2">數</div>
</body>
</html>
