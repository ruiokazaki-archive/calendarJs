<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="ress.css" />
    <link rel="stylesheet" href="style.css" />
    <title>sample</title>
  </head>

  <body>
    <div class="calendar">
      <h4 id="title"></h4>
      <div class="btns">
        <button id="back">‹</button>
        <button id="next">›</button>
      </div>
      <table class="calendar__table" id="calendar" data-lang="ja">
        <thead id="calendar__thead"></thead>
        <tbody id="calendar__tbody"></tbody>
      </table>
      <div class="selects">
        <label for="month">日付指定：</label>
        <select id="month">
          <option value="0">1月</option>
          <option value="1">2月</option>
          <option value="2">3月</option>
          <option value="3">4月</option>
          <option value="4">5月</option>
          <option value="5">6月</option>
          <option value="6">7月</option>
          <option value="7">8月</option>
          <option value="8">9月</option>
          <option value="9">10月</option>
          <option value="10">11月</option>
          <option value="11">12月</option>
        </select>
        <select id="year"></select>
      </div>
    </div>
    <script src="script.js"></script>
  </body>
</html>
