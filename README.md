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
    <style>
            /*!
       * ress.css • v1.1.2
       * MIT License
       * github.com/filipelinhares/ress
       */

      /\* # =================================================================

      # Global selectors

      # ================================================================= \*/

      html {
      box-sizing: border-box;
      overflow-y: scroll; /_ All browsers without overlaying scrollbars _/
      -webkit-text-size-adjust: 100%; /_ iOS 8+ _/
      }

      \*,
      ::before,
      ::after {
      box-sizing: inherit;
      }

      ::before,
      ::after {
      text-decoration: inherit; /_ Inherit text-decoration and vertical align to ::before and ::after pseudo elements _/
      vertical-align: inherit;
      }

      /_ Remove margin, padding of all elements and set background-no-repeat as default _/

      - {
        background-repeat: no-repeat; /_ Set `background-repeat: no-repeat` to all elements _/
        padding: 0; /_ Reset `padding` and `margin` of all elements _/
        margin: 0;
        }

      /\* # =================================================================

      # General elements

      # ================================================================= \*/

      /_ Add the correct display in iOS 4-7._/
      audio:not([controls]) {
      display: none;
      height: 0;
      }

      hr {
      overflow: visible; /_ Show the overflow in Edge and IE _/
      }

      /\*

      - Correct `block` display not defined for any HTML5 element in IE 8/9
      - Correct `block` display not defined for `details` or `summary` in IE 10/11
      - and Firefox
      - Correct `block` display not defined for `main` in IE 11
        \*/
        article,
        aside,
        details,
        figcaption,
        figure,
        footer,
        header,
        main,
        menu,
        nav,
        section,
        summary {
        display: block;
        }

      summary {
      display: list-item; /_ Add the correct display in all browsers _/
      }

      small {
      font-size: 80%; /_ Set font-size to 80% in `small` elements _/
      }

      [hidden],
      template {
      display: none; /_ Add the correct display in IE _/
      }

      abbr[title] {
      border-bottom: 1px dotted; /_ Add a bordered underline effect in all browsers _/
      text-decoration: none; /_ Remove text decoration in Firefox 40+ _/
      }

      a {
      background-color: transparent; /_ Remove the gray background on active links in IE 10 _/
      -webkit-text-decoration-skip: objects; /_ Remove gaps in links underline in iOS 8+ and Safari 8+ _/
      }

      a:active,
      a:hover {
      outline-width: 0; /_ Remove the outline when hovering in all browsers _/
      }

      code,
      kbd,
      pre,
      samp {
      font-family: monospace, monospace; /_ Specify the font family of code elements _/
      }

      b,
      strong {
      font-weight: bolder; /_ Correct style set to `bold` in Edge 12+, Safari 6.2+, and Chrome 18+ _/
      }

      dfn {
      font-style: italic; /_ Address styling not present in Safari and Chrome _/
      }

      /_ Address styling not present in IE 8/9 _/
      mark {
      background-color: #ff0;
      color: #000;
      }

      /_ https://gist.github.com/unruthless/413930 _/
      sub,
      sup {
      font-size: 75%;
      line-height: 0;
      position: relative;
      vertical-align: baseline;
      }

      sub {
      bottom: -0.25em;
      }

      sup {
      top: -0.5em;
      }

      /\* # =================================================================

      # Forms

      # ================================================================= \*/

      input {
      border-radius: 0;
      }

      /_ Apply cursor pointer to button elements _/
      button,
      [type="button"],
      [type="reset"],
      [type="submit"],
      [role="button"] {
      cursor: pointer;
      }

      /_ Replace pointer cursor in disabled elements _/
      [disabled] {
      cursor: default;
      }

      [type="number"] {
      width: auto; /_ Firefox 36+ _/
      }

      [type="search"] {
      -webkit-appearance: textfield; /_ Safari 8+ _/
      }

      [type="search"]: :-webkit-search-cancel-button,

      [type="search"]::-webkit-search-decoration {
      -webkit-appearance: none; /_ Safari 8 _/
      }

      textarea {
      overflow: auto; /_ Internet Explorer 11+ _/
      resize: vertical; /_ Specify textarea resizability _/
      }

      button,
      input,
      optgroup,
      select,
      textarea {
      font: inherit; /_ Specify font inheritance of form elements _/
      }

      optgroup {
      font-weight: bold; /_ Restore the font weight unset by the back rule. _/
      }

      button {
      overflow: visible; /_ Address `overflow` set to `hidden` in IE 8/9/10/11 _/
      }

      /_ Remove inner padding and border in Firefox 4+ _/
      button::-moz-focus-inner,
      [type="button"]::-moz-focus-inner,
      [type="reset"]::-moz-focus-inner,
      [type="submit"]::-moz-focus-inner {
      border-style: 0;
      padding: 0;
      }

      /_ Replace focus style removed in the border reset above _/
      button:-moz-focusring,
      [type="button"]::-moz-focus-inner,
      [type="reset"]::-moz-focus-inner,
      [type="submit"]::-moz-focus-inner {
      outline: 1px dotted ButtonText;
      }

      button,
      html [type="button"], /_ Prevent a WebKit bug where (2) destroys native `audio` and `video`controls in Android 4 _/
      [type="reset"],
      [type="submit"] {
      -webkit-appearance: button; /_ Correct the inability to style clickable types in iOS _/
      }

      button,
      select {
      text-transform: none; /_ Firefox 40+, Internet Explorer 11- _/
      }

      /_ Remove the default button styling in all browsers _/
      button,
      input,
      select,
      textarea {
      background-color: transparent;
      border-style: none;
      color: inherit;
      }

      /_ Style select like a standard input _/
      select {
      -moz-appearance: none; /_ Firefox 36+ _/
      -webkit-appearance: none; /_ Chrome 41+ _/
      }

      select::-ms-expand {
      display: none; /_ Internet Explorer 11+ _/
      }

      select::-ms-value {
      color: currentColor; /_ Internet Explorer 11+ _/
      }

      legend {
      border: 0; /_ Correct `color` not being inherited in IE 8/9/10/11 _/
      color: inherit; /_ Correct the color inheritance from `fieldset` elements in IE _/
      display: table; /_ Correct the text wrapping in Edge and IE _/
      max-width: 100%; /_ Correct the text wrapping in Edge and IE _/
      white-space: normal; /_ Correct the text wrapping in Edge and IE _/
      }

      ::-webkit-file-upload-button {
      -webkit-appearance: button; /_ Correct the inability to style clickable types in iOS and Safari _/
      font: inherit; /_ Change font properties to `inherit` in Chrome and Safari _/
      }

      [type="search"] {
      -webkit-appearance: textfield; /_ Correct the odd appearance in Chrome and Safari _/
      outline-offset: -2px; /_ Correct the outline style in Safari _/
      }

      /\* # =================================================================

      # Specify media element style

      # ================================================================= \*/

      img {
      border-style: none; /_ Remove border when inside `a` element in IE 8/9/10 _/
      }

      /_ Add the correct vertical alignment in Chrome, Firefox, and Opera _/
      progress {
      vertical-align: baseline;
      }

      svg:not(:root) {
      overflow: hidden; /_ Internet Explorer 11- _/
      }

      audio,
      canvas,
      progress,
      video {
      display: inline-block; /_ Internet Explorer 11+, Windows Phone 8.1+ _/
      }

      /\* # =================================================================

      # Accessibility

      # ================================================================= \*/

      /_ Hide content from screens but not screenreaders _/
      @media screen {
      [hidden~="screen"] {
      display: inherit;
      }
      [hidden~="screen"]:not(:active):not(:focus):not(:target) {
      position: absolute !important;
      clip: rect(0 0 0 0) !important;
      }
      }

      /_ Specify the progress cursor of updating elements _/
      [aria-busy="true"] {
      cursor: progress;
      }

      /_ Specify the pointer cursor of trigger elements _/
      [aria-controls] {
      cursor: pointer;
      }

      /_ Specify the unstyled cursor of disabled, not-editable, or otherwise inoperable elements _/
      [aria-disabled] {
      cursor: default;
      }

      /\* # =================================================================

      # Selection

      # ================================================================= \*/

      /_ Specify text selection background color and omit drop shadow _/

      ::-moz-selection {
      background-color: #b3d4fc; /_ Required when declaring ::selection _/
      color: #000;
      text-shadow: none;
      }

      ::selection {
      background-color: #b3d4fc; /_ Required when declaring ::selection _/
      color: #000;
      text-shadow: none;
      }
    </style>
    <style>
      .calendar {
        background: #ffffff;
        padding: 15px;
        width: 100%;
        margin: 0 auto;
        overflow: auto;
      }
      .btns button {
        cursor: pointer;
        display: inline-block;
        zoom: 1;
        background: pink;
        color: #fff;
        border-radius: 4px;
        padding: 5px 10px;
      }
      .calendar**table {
        border-collapse: collapse;
        width: min-content;
      }
      .calendar**table th,
      .calendar\_\_table td {
        padding: 10px;
        border: 1px solid #e2e2e2;
        text-align: center;
        vertical-align: top;
      }
      .date-picker.selected {
        font-weight: bold;
        color: #fff;
        background: pink;
      }
      #title {
        text-align: center;
        width: 300px;
      }
      .btns {
        margin-bottom: 1em;
        overflow: hidden;
        width: 300px;
        display: flex;
        justify-content: space-between;
      }
      .selects {
        margin-top: 1em;
        border-top: 1px solid #dadada;
        padding: 10px 0;
      }
      .selects select {
        cursor: pointer;
        display: inline-block;
        zoom: 1;
        background: #ffffff;
        color: #454545;
        border: 1px solid #bfc5c5;
        border-radius: 3px;
        padding: 5px 1em;
      }
      .date-picker.selected span {
        border-bottom: 2px solid white;
      }
    </style>
    <script>
      const today = new Date();
      let currentMonth = today.getMonth();
      let currentYear = today.getFullYear();
      const selectYear = document.getElementById("year");
      const selectMonth = document.getElementById("month");
      const next = document.getElementById("next");
      const back = document.getElementById("back");
      const month = document.getElementById("month");
      const year = document.getElementById("year");
      const thead = document.getElementById("calendar__thead");
      const tbody = document.getElementById("calendar__tbody");
      const months = [
        "1月",
        "2月",
        "3月",
        "4月",
        "5月",
        "6月",
        "7月",
        "8月",
        "9月",
        "10月",
        "11月",
        "12月",
      ];
      const days = ["日", "月", "火", "水", "木", "金", "土"];
      let createYear = generate_year_range(1900, 2100);
      let calendar = document.getElementById("calendar");
      let lang = calendar.getAttribute("data-lang");

      document.getElementById("year").innerHTML = createYear;

      let dayHeader = "<tr>";
      for (day in days) {
        dayHeader += "<th data-days='" + days[day] + "'>" + days[day] + "</th>";
      }
      dayHeader += "</tr>";
      thead.innerHTML = dayHeader;

      const title = document.getElementById("title");
      showCalendar(currentMonth, currentYear);
      next.addEventListener("click", () => {
        currentYear = currentMonth === 11 ? currentYear + 1 : currentYear;
        currentMonth = (currentMonth + 1) % 12;
        showCalendar(currentMonth, currentYear);
      });
      back.addEventListener("click", () => {
        currentYear = currentMonth === 0 ? currentYear - 1 : currentYear;
        currentMonth = currentMonth === 0 ? 11 : currentMonth - 1;
        showCalendar(currentMonth, currentYear);
      });
      month.addEventListener("change", () => {
        currentYear = parseInt(selectYear.value);
        currentMonth = parseInt(selectMonth.value);
        showCalendar(currentMonth, currentYear);
      });
      year.addEventListener("change", () => {
        currentYear = parseInt(selectYear.value);
        currentMonth = parseInt(selectMonth.value);
        showCalendar(currentMonth, currentYear);
      });

      function showCalendar(month, year) {
        let firstDay = new Date(year, month).getDay();

        tbody.innerHTML = "";

        title.innerHTML = year + "年" + "　" + months[month];
        selectYear.value = year;
        selectMonth.value = month;

        // creating all cells
        let date = 1;
        for (let i = 0; i < 6; i++) {
          let row = document.createElement("tr");

          for (let j = 0; j < 7; j++) {
            if (i === 0 && j < firstDay) {
              cell = document.createElement("td");
              cellText = document.createTextNode("");
              cell.appendChild(cellText);
              row.appendChild(cell);
            } else if (date > daysInMonth(month, year)) {
              break;
            } else {
              cell = document.createElement("td");
              cell.setAttribute("data-date", date);
              cell.setAttribute("data-month", month + 1);
              cell.setAttribute("data-year", year);
              cell.setAttribute("data-month_name", months[month]);
              cell.className = "date-picker";
              cell.innerHTML = "<span>" + date + "</span>";

              if (
                date === today.getDate() &&
                year === today.getFullYear() &&
                month === today.getMonth()
              ) {
                cell.className = "date-picker selected";
              }
              row.appendChild(cell);
              date++;
            }
          }

          tbody.appendChild(row);
        }
      }

      function daysInMonth(iMonth, iYear) {
        return 32 - new Date(iYear, iMonth, 32).getDate();
      }

      function generate_year_range(start, end) {
        let years = "";
        for (let year = start; year <= end; year++) {
          years += "<option value='" + year + "'>" + year + "</option>";
        }
        return years;
      }
    </script>
