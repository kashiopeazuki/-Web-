<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>発車メロディースイッチ</title>
<style>
  .button {
    padding: 20px 40px;
    font-size: 20px;
    cursor: pointer;
    background-color: #f00; /* 赤色スイッチ */
    color: white;
    border-radius: 10px;
    border: none;
    box-shadow: 0 5px #990000;
  }
  .button:active {
    box-shadow: 0 2px #990000;
    transform: translateY(3px);
  }
</style>
</head>
<body>

<button class="button" onclick="playMelody()">発車メロディー</button>

<script>
  function playMelody() {
    // 音声ファイルのパス（適宜変更してください）
    const audio = new Audio('melody.mp3');
    audio.play();
  }
</script>

</body>
</html>
