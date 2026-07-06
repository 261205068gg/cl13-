<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="utf-8">
  <title>花畑の朝</title>
  <style>
    /* 全体の配置を決めるボックス */
    .container {
      position: relative;
      width: 1000px;       /* 見本の横幅に合わせて調整してください */
      height: 600px;       /* 見本の縦幅に合わせて調整してください */
      overflow: hidden;
    }

    /* 背景の家と花畑の画像 */
    .background-img {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: 1;          /* 一番後ろ */
    }

    /* 左上の文字が入る白い半透明のボックス */
    .text-box {
      position: absolute;
      top: 60px;           /* 上からの位置 */
      left: 50px;          /* 左からの位置 */
      background-color: rgba(255, 255, 255, 0.6); /* 白色の半透明（0.6） */
      padding: 15px 25px;  /* 内側の余白 */
      border-radius: 4px;  /* 角を少し丸くする */
      z-index: 10;         /* 画像より前に出す */
    }

    /* ボックスの中の文字（ピンク・赤系の色） */
    .text-box p {
      margin: 0;
      font-size: 24px;     /* 文字の大きさ */
      font-weight: bold;   /* 太字 */
      color: #d13264;      /* 見本に近いピンク・赤系の色 */
      line-height: 1.5;    /* 行の間隔 */
    }

    /* 蝶々の画像（位置の例：1匹目） */
    .butterfly1 {
      position: absolute;
      bottom: 80px;        /* 下からの位置 */
      left: 180px;         /* 左からの位置 */
      width: 80px;         /* 蝶のサイズ（お好みで変更してください） */
      z-index: 5;          /* 背景より前、文字より後ろ */
    }

    /* 蝶々の画像（位置の例：2匹目） */
    .butterfly2 {
      position: absolute;
      bottom: 120px;
      left: 400px;
      width: 75px;
      z-index: 5;
    }

    /* 蝶々の画像（位置の例：3匹目） */
    .butterfly3 {
      position: absolute;
      bottom: 60px;
      right: 250px;
      width: 85px;
      z-index: 5;
    }

    /* 右下の小さな白い文字（クレジット） */
    .credit-text {
      position: absolute;
      bottom: 15px;
      right: 20px;
      color: #ffffff;      /* 白色 */
      font-size: 14px;
      margin: 0;
      z-index: 10;
    }
  </style>
</head>
<body>

<div class="container">
  <!-- 背景画像（ファイル名は実際の物に変えてください） -->
  <img src="./bg_house.png" class="background-img" alt="背景">

  <!-- 左上の文字部分 -->
  <div class="text-box">
    <p>ぽかぽか陽気の穏やかな朝<br>花畑では、蝶々がのんびり飛んでいます</p>
  </div>

  <!-- 蝶々の画像（ファイル名や位置は調整してください） -->
  <img src="./butterfly.png" class="butterfly1" alt="蝶1">
  <img src="./butterfly.png" class="butterfly2" alt="蝶2">
  <img src="./butterfly.png" class="butterfly3" alt="蝶3">

  <!-- 右下のクレジット文字 -->
  <p class="credit-text">このイラストは、Adobe Firefly Image 5 で生成しました</p>
</div>

</body>
</html>
