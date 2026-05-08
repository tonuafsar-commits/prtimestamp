<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>PRTimestamp - Premiere Pro Timestamp Shortcut CSV Converter</title>
    <meta name="description" content="PRTimestamp converts Premiere Pro marker CSV exports into clean timestamps for YouTube chapters, notes, captions, and edit reviews.">
    <meta name="keywords" content="premiere pro timestamp shortcut, premiere timestamp shortcut, premiere pro marker export, premiere pro csv markers, youtube chapters premiere pro, prtimestamp">
    <meta name="robots" content="index, follow">
    <meta property="og:title" content="PRTimestamp - Premiere Pro Timestamp Shortcut">
    <meta property="og:description" content="Convert Premiere Pro marker CSV exports into clean timestamp text for YouTube chapters, notes, and captions.">
    <meta property="og:type" content="website">
    <style>
      :root {
        color-scheme: dark;
        --bg: #09111f;
        --panel: #101827;
        --panel-2: #142033;
        --panel-3: #0c1422;
        --text: #eef4ff;
        --muted: #9fb0c7;
        --line: #29384f;
        --accent: #2dd4bf;
        --accent-2: #f59e0b;
        --danger: #fb7185;
        --button-text: #04110f;
      }

      * {
        box-sizing: border-box;
      }

      body {
        margin: 0;
        min-height: 100vh;
        background:
          radial-gradient(circle at 8% 4%, rgba(45, 212, 191, 0.18), transparent 28%),
          linear-gradient(135deg, #09111f 0%, #111827 52%, #0b1220 100%);
        color: var(--text);
        font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      }

      button,
      input,
      select,
      textarea {
        font: inherit;
      }

      button {
        min-height: 40px;
        border: 0;
        border-radius: 6px;
        background: var(--accent);
        color: var(--button-text);
        font-weight: 800;
        padding: 0 14px;
        cursor: pointer;
      }

      button:hover:not(:disabled) {
        filter: brightness(1.08);
      }

      button:disabled {
        cursor: not-allowed;
        opacity: 0.46;
      }

      input,
      select,
      textarea {
        width: 100%;
        border: 1px solid var(--line);
        border-radius: 6px;
        background: var(--panel-3);
        color: var(--text);
        padding: 10px 11px;
      }

      select {
        min-height: 40px;
      }

      textarea {
        min-height: 280px;
        resize: vertical;
        line-height: 1.5;
        font-family: Consolas, "Liberation Mono", monospace;
        font-size: 0.94rem;
      }

      input:focus,
      select:focus,
      textarea:focus,
      button:focus-visible {
        outline: 2px solid rgba(45, 212, 191, 0.62);
        outline-offset: 2px;
      }

      .app-shell {
        width: min(1220px, calc(100% - 28px));
        margin: 0 auto;
        padding: 28px 0;
      }

      .workspace {
        display: grid;
        gap: 18px;
        min-height: calc(100vh - 56px);
        border: 1px solid rgba(159, 176, 199, 0.18);
        border-radius: 8px;
        background: rgba(16, 24, 39, 0.96);
        padding: clamp(16px, 2.6vw, 28px);
      }

      .topbar,
      .toolbar,
      .preview-heading,
      .status-row,
      .inline-actions {
        display: flex;
        align-items: center;
        gap: 12px;
      }

      .topbar,
      .preview-heading,
      .status-row {
        justify-content: space-between;
      }

      .eyebrow {
        margin: 0 0 6px;
        color: var(--accent);
        font-size: 0.78rem;
        font-weight: 800;
        letter-spacing: 0;
        text-transform: uppercase;
      }

      h1,
      h2,
      p {
        margin: 0;
        letter-spacing: 0;
      }

      h1 {
        font-size: clamp(1.55rem, 2.6vw, 2.45rem);
        line-height: 1.08;
      }

      h2 {
        font-size: 1rem;
      }

      .ghost-button {
        border: 1px solid var(--line);
        background: #0b1320;
        color: var(--text);
      }

      .main-grid {
        display: grid;
        grid-template-columns: minmax(0, 0.88fr) minmax(360px, 1.12fr);
        gap: 18px;
        align-items: start;
      }

      .how-to {
        border: 1px solid rgba(245, 158, 11, 0.62);
        border-radius: 8px;
        background: linear-gradient(135deg, rgba(245, 158, 11, 0.18), rgba(45, 212, 191, 0.1));
        padding: 16px;
      }

      .how-to h2 {
        color: #fef3c7;
        font-size: 1.08rem;
        margin-bottom: 10px;
      }

      .how-to p {
        color: #f8fafc;
        line-height: 1.55;
      }

      .how-to p + p {
        margin-top: 8px;
      }

      .panel {
        border: 1px solid var(--line);
        border-radius: 8px;
        background: var(--panel-2);
        padding: 16px;
      }

      .drop-zone {
        display: grid;
        gap: 7px;
        place-items: center;
        min-height: 150px;
        border: 2px dashed #49607e;
        border-radius: 8px;
        background: #0d1727;
        text-align: center;
        cursor: pointer;
        transition: border-color 160ms ease, background 160ms ease, transform 160ms ease;
      }

      .drop-zone:hover,
      .drop-zone.is-dragging {
        border-color: var(--accent);
        background: #0b1f27;
      }

      .drop-zone.is-dragging {
        transform: scale(1.01);
      }

      .drop-zone input {
        position: absolute;
        inline-size: 1px;
        block-size: 1px;
        opacity: 0;
        pointer-events: none;
      }

      .drop-title {
        font-weight: 800;
      }

      .drop-meta,
      .status,
      .metric-label,
      label {
        color: var(--muted);
        font-size: 0.9rem;
      }

      .field-grid {
        display: grid;
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 12px;
        margin-top: 14px;
      }

      .field-grid .wide {
        grid-column: 1 / -1;
      }

      label {
        display: grid;
        gap: 7px;
        font-weight: 700;
      }

      .toolbar {
        flex-wrap: wrap;
        margin-top: 14px;
      }

      .metrics {
        display: grid;
        grid-template-columns: repeat(3, minmax(0, 1fr));
        gap: 10px;
        margin-top: 14px;
      }

      .metric {
        min-height: 76px;
        border: 1px solid rgba(159, 176, 199, 0.16);
        border-radius: 8px;
        background: rgba(12, 20, 34, 0.72);
        padding: 12px;
      }

      .metric-value {
        display: block;
        color: var(--accent);
        font-size: 1.7rem;
        font-weight: 800;
        line-height: 1;
      }

      .status-row {
        min-height: 28px;
      }

      .support-link {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        min-height: 52px;
        border: 1px solid rgba(245, 158, 11, 0.7);
        border-radius: 8px;
        background: linear-gradient(135deg, rgba(245, 158, 11, 0.24), rgba(45, 212, 191, 0.18));
        color: #fef3c7;
        font-size: clamp(1.05rem, 2.2vw, 1.45rem);
        font-weight: 700;
        padding: 12px 18px;
        text-decoration: none;
        width: 100%;
      }

      .support-link:hover {
        border-color: var(--accent-2);
        background: linear-gradient(135deg, rgba(245, 158, 11, 0.34), rgba(45, 212, 191, 0.25));
        text-decoration: underline;
      }

      .signature {
        color: #fef3c7;
        font-family: "Brush Script MT", "Segoe Script", "Lucida Handwriting", cursive;
        font-size: clamp(1.8rem, 4vw, 3rem);
        line-height: 1;
        text-align: center;
        text-shadow: 0 0 18px rgba(245, 158, 11, 0.36);
      }

      .status {
        min-width: 0;
      }

      .status.error {
        color: var(--danger);
        font-weight: 800;
      }

      .status.warning {
        color: var(--accent-2);
        font-weight: 800;
      }

      .paste-input {
        min-height: 170px;
        margin-top: 14px;
      }

      .preview-table-wrap {
        max-height: 230px;
        overflow: auto;
        border: 1px solid var(--line);
        border-radius: 8px;
        background: var(--panel-3);
      }

      table {
        width: 100%;
        border-collapse: collapse;
        font-size: 0.88rem;
      }

      th,
      td {
        max-width: 260px;
        border-bottom: 1px solid rgba(159, 176, 199, 0.14);
        padding: 9px 10px;
        text-align: left;
        vertical-align: top;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
      }

      th {
        position: sticky;
        top: 0;
        z-index: 1;
        background: #0f1b2c;
        color: var(--muted);
      }

      .output-panel {
        display: grid;
        gap: 12px;
      }

      .output-panel textarea {
        min-height: 430px;
      }

      .hint {
        color: var(--muted);
        font-size: 0.84rem;
      }

      @media (max-width: 920px) {
        .main-grid,
        .field-grid {
          grid-template-columns: 1fr;
        }

        .field-grid .wide {
          grid-column: auto;
        }
      }

      @media (max-width: 680px) {
        .topbar,
        .preview-heading,
        .status-row,
        .inline-actions {
          align-items: stretch;
          flex-direction: column;
        }

        .toolbar,
        .metrics {
          grid-template-columns: 1fr;
        }

        button {
          width: 100%;
        }
      }
    </style>
  </head>
  <body>
    <main class="app-shell">
      <section class="workspace" aria-labelledby="app-title">
        <header class="topbar">
          <div>
            <p class="eyebrow">Premiere CSV to timestamps</p>
            <h1 id="app-title">PRTimestamp</h1>
          </div>
          <div class="inline-actions">
            <button class="ghost-button" id="sampleButton" type="button">Load Sample</button>
            <button class="ghost-button" id="clearButton" type="button">Clear</button>
          </div>
        </header>

        <section class="how-to" aria-labelledby="how-to-title">
          <h2 id="how-to-title">How to Use</h2>
          <p>Mark your desired points and give each marker a name <em>(to add a name, press the marker shortcut <strong>M</strong> again)</em>.</p>
          <p>Once you’ve added all markers and names, go to the <strong>Export</strong> option in Premiere Pro. Choose where you want to save the marker export.</p>
          <p>It will be saved as a <strong>.csv file</strong> with your project name.</p>
          <p>Now just upload that CSV file… and voilà, you’re done! 🎉</p>
        </section>

        <div class="main-grid">
          <section class="panel" aria-label="CSV input and settings">
            <label class="drop-zone" id="dropZone">
              <input id="csvFile" type="file" accept=".csv,.tsv,text/csv,text/tab-separated-values,text/plain">
              <span class="drop-title" id="dropTitle">Choose CSV or TSV</span>
              <span class="drop-meta" id="dropMeta">Drop a marker export here</span>
            </label>

            <textarea class="paste-input" id="rawInput" spellcheck="false" placeholder="Paste CSV here, then click Parse Paste."></textarea>

            <div class="toolbar">
              <button id="parsePasteButton" type="button">Parse Paste</button>
              <button class="ghost-button" id="copyInputButton" type="button">Copy Input</button>
            </div>

            <div class="field-grid">
              <label>
                Time column
                <select id="timeColumn"></select>
              </label>
              <label>
                Comment column
                <select id="commentColumn"></select>
              </label>
              <label>
                Output format
                <select id="formatMode">
                  <option value="standard">MM:SS - Comment</option>
                  <option value="hours">HH:MM:SS - Comment</option>
                  <option value="youtube">MM:SS Comment</option>
                  <option value="chapters">YouTube chapters</option>
                  <option value="srt">SRT captions</option>
                </select>
              </label>
              <label>
                Sort
                <select id="sortMode">
                  <option value="file">Keep file order</option>
                  <option value="time">Sort by time</option>
                </select>
              </label>
              <label class="wide">
                Fallback comment columns
                <input id="fallbackColumns" type="text" placeholder="Auto-detected after load">
              </label>
            </div>

            <div class="toolbar">
              <button id="convertButton" type="button" disabled>Convert</button>
              <button class="ghost-button" id="downloadButton" type="button" disabled>Download TXT</button>
              <button class="ghost-button" id="copyOutputButton" type="button" disabled>Copy Output</button>
            </div>

            <div class="metrics" aria-label="CSV summary">
              <div class="metric">
                <span class="metric-value" id="rowCount">0</span>
                <span class="metric-label">rows</span>
              </div>
              <div class="metric">
                <span class="metric-value" id="validCount">0</span>
                <span class="metric-label">valid times</span>
              </div>
              <div class="metric">
                <span class="metric-value" id="skippedCount">0</span>
                <span class="metric-label">skipped</span>
              </div>
            </div>
          </section>

          <section class="output-panel">
            <div class="panel">
              <div class="preview-heading">
                <h2>Data Preview</h2>
                <span class="hint" id="delimiterLabel">No file loaded</span>
              </div>
              <div class="preview-table-wrap" id="previewWrap">
                <table id="previewTable">
                  <thead><tr><th>Waiting for input</th></tr></thead>
                  <tbody><tr><td>Load or paste a CSV to preview rows.</td></tr></tbody>
                </table>
              </div>
            </div>

            <div class="panel">
              <div class="preview-heading">
                <h2>Output</h2>
                <span class="hint" id="lineCount">0 lines</span>
              </div>
              <textarea id="output" spellcheck="false" placeholder="Converted timestamps will appear here."></textarea>
            </div>
          </section>
        </div>

        <div class="status-row">
          <p class="status" id="status" role="status">Waiting for a Premiere marker export.</p>
          <span class="hint">Shortcuts: Ctrl/⌘+Enter converts, Ctrl/⌘+S downloads.</span>
        </div>

        <div class="status-row">
          <a class="support-link" href="https://youtu.be/Aq5WXmQQooo?si=kkiAeYRY9M_koSpZ" target="_blank" rel="noopener noreferrer">Your support means a lot — watch the full video</a>
        </div>

        <div class="signature" aria-label="Signature">ANTonmoy</div>
      </section>
    </main>

    <script>
      const fileInput = document.getElementById("csvFile");
      const dropZone = document.getElementById("dropZone");
      const dropTitle = document.getElementById("dropTitle");
      const dropMeta = document.getElementById("dropMeta");
      const rawInput = document.getElementById("rawInput");
      const timeColumn = document.getElementById("timeColumn");
      const commentColumn = document.getElementById("commentColumn");
      const formatMode = document.getElementById("formatMode");
      const sortMode = document.getElementById("sortMode");
      const fallbackColumns = document.getElementById("fallbackColumns");
      const convertButton = document.getElementById("convertButton");
      const downloadButton = document.getElementById("downloadButton");
      const copyOutputButton = document.getElementById("copyOutputButton");
      const copyInputButton = document.getElementById("copyInputButton");
      const parsePasteButton = document.getElementById("parsePasteButton");
      const sampleButton = document.getElementById("sampleButton");
      const clearButton = document.getElementById("clearButton");
      const statusBox = document.getElementById("status");
      const output = document.getElementById("output");
      const lineCount = document.getElementById("lineCount");
      const rowCount = document.getElementById("rowCount");
      const validCount = document.getElementById("validCount");
      const skippedCount = document.getElementById("skippedCount");
      const delimiterLabel = document.getElementById("delimiterLabel");
      const previewTable = document.getElementById("previewTable");

      const timeCandidates = [
        "timecode",
        "time code",
        "start tc",
        "start",
        "marker start",
        "in",
        "position",
        "time",
      ];
      const commentCandidates = [
        "comment",
        "comments",
        "description",
        "marker name",
        "name",
        "note",
        "notes",
        "text",
      ];

      let rows = [];
      let headers = [];
      let outputText = "";
      let sourceName = "premiere-timestamps";
      let detectedFallbacks = [];
      const markerDescriptionOption = "__marker_name_description";

      function setStatus(message, tone = "normal") {
        statusBox.textContent = message;
        statusBox.classList.toggle("error", tone === "error");
        statusBox.classList.toggle("warning", tone === "warning");
      }

      function decodeTextBuffer(buffer) {
        const bytes = new Uint8Array(buffer);

        if (bytes[0] === 0xff && bytes[1] === 0xfe) {
          return new TextDecoder("utf-16le").decode(buffer);
        }

        if (bytes[0] === 0xfe && bytes[1] === 0xff) {
          return new TextDecoder("utf-16be").decode(buffer);
        }

        const sample = bytes.slice(0, 240);
        const oddZeroes = Array.from(sample).filter((byte, index) => index % 2 === 1 && byte === 0).length;
        if (sample.length > 0 && oddZeroes > sample.length * 0.28) {
          return new TextDecoder("utf-16le").decode(buffer);
        }

        return new TextDecoder("utf-8").decode(buffer).replace(/^\uFEFF/, "");
      }

      function countDelimiterOutsideQuotes(text, delimiter) {
        let count = 0;
        let inQuotes = false;

        for (let i = 0; i < text.length; i += 1) {
          const char = text[i];
          const next = text[i + 1];

          if (char === '"' && inQuotes && next === '"') {
            i += 1;
          } else if (char === '"') {
            inQuotes = !inQuotes;
          } else if (char === delimiter && !inQuotes) {
            count += 1;
          }
        }

        return count;
      }

      function detectDelimiter(text) {
        const sample = text.slice(0, 12000);
        const candidates = [",", "\t", ";"];
        return candidates
          .map((delimiter) => ({
            delimiter,
            count: countDelimiterOutsideQuotes(sample, delimiter),
          }))
          .sort((a, b) => b.count - a.count)[0].delimiter;
      }

      function parseCsv(text, delimiter) {
        const records = [];
        let row = [];
        let value = "";
        let inQuotes = false;

        for (let i = 0; i < text.length; i += 1) {
          const char = text[i];
          const next = text[i + 1];

          if (char === '"' && inQuotes && next === '"') {
            value += '"';
            i += 1;
          } else if (char === '"') {
            inQuotes = !inQuotes;
          } else if (char === delimiter && !inQuotes) {
            row.push(value.trim());
            value = "";
          } else if ((char === "\n" || char === "\r") && !inQuotes) {
            if (char === "\r" && next === "\n") {
              i += 1;
            }
            row.push(value.trim());
            if (row.some((cell) => cell !== "")) {
              records.push(row);
            }
            row = [];
            value = "";
          } else {
            value += char;
          }
        }

        if (inQuotes) {
          throw new Error("A quoted CSV field is missing its closing quote.");
        }

        row.push(value.trim());
        if (row.some((cell) => cell !== "")) {
          records.push(row);
        }

        return records;
      }

      function makeUniqueHeaders(headerRow) {
        const seen = new Map();

        return headerRow.map((header, index) => {
          const fallback = `Column ${index + 1}`;
          const base = String(header || fallback).trim().replace(/^\uFEFF/, "") || fallback;
          const count = seen.get(base.toLowerCase()) || 0;
          seen.set(base.toLowerCase(), count + 1);
          return count === 0 ? base : `${base} (${count + 1})`;
        });
      }

      function recordsToObjects(records) {
        const cleanHeaders = makeUniqueHeaders(records[0] || []);
        const dataRows = records.slice(1);

        return {
          headers: cleanHeaders,
          rows: dataRows.map((cells, index) => {
            const item = { __rowNumber: index + 2 };
            cleanHeaders.forEach((header, cellIndex) => {
              item[header] = String(cells[cellIndex] || "").trim();
            });
            return item;
          }),
        };
      }

      function extractSeconds(value) {
        const timecode = String(value || "")
          .trim()
          .replace(/[,;](\d{1,3})$/, ":$1");
        const parts = timecode.split(":");
        const numberOnly = timecode.match(/^(\d+(?:\.\d+)?)s?$/i);

        if (numberOnly) {
          return Math.max(0, Number(numberOnly[1]));
        }

        if (!parts.every((part) => /^\d+(?:\.\d+)?$/.test(part))) {
          return null;
        }

        if (parts.length === 2) {
          const [mm, ss] = parts.map(Number);
          return mm * 60 + ss;
        }

        if (parts.length === 3) {
          const [hh, mm, ss] = parts.map(Number);
          return hh * 3600 + mm * 60 + ss;
        }

        if (parts.length >= 4) {
          const [hh, mm, ss] = parts.map(Number);
          return hh * 3600 + mm * 60 + ss;
        }

        return null;
      }

      function formatSeconds(totalSeconds, mode) {
        const rounded = Math.max(0, Math.floor(Number(totalSeconds) || 0));
        const hh = Math.floor(rounded / 3600);
        const mm = Math.floor((rounded % 3600) / 60);
        const ss = rounded % 60;

        if (mode === "hours" || mode === "srt") {
          return `${String(hh).padStart(2, "0")}:${String(mm).padStart(2, "0")}:${String(ss).padStart(2, "0")}`;
        }

        return `${String(mm + hh * 60).padStart(2, "0")}:${String(ss).padStart(2, "0")}`;
      }

      function formatSrtTime(totalSeconds) {
        return `${formatSeconds(totalSeconds, "hours")},000`;
      }

      function detectColumn(fieldNames, possibleNames, blockedColumn = "") {
        const available = fieldNames.filter((field) => field !== blockedColumn);
        const exact = possibleNames
          .map((name) => available.find((field) => field.trim().toLowerCase() === name))
          .find(Boolean);

        if (exact) {
          return exact;
        }

        return possibleNames
          .map((name) => available.find((field) => field.toLowerCase().includes(name)))
          .find(Boolean) || "";
      }

      function scoreTimeColumn(column) {
        return rows.reduce((score, row) => score + (extractSeconds(row[column]) !== null ? 1 : 0), 0);
      }

      function detectTimeColumn() {
        const scored = headers
          .map((header) => ({ header, score: scoreTimeColumn(header) }))
          .sort((a, b) => b.score - a.score);

        if (scored[0] && scored[0].score > 0) {
          return scored[0].header;
        }

        return detectColumn(headers, timeCandidates);
      }

      function detectCommentColumn(timeColumnName) {
        const markerName = headers.find((header) => (
          header !== timeColumnName &&
          header.trim().toLowerCase() === "marker name"
        ));

        if (markerName) {
          return markerName;
        }

        const headerMatch = detectColumn(headers, commentCandidates, timeColumnName);

        if (headerMatch) {
          return headerMatch;
        }

        return headers
          .filter((header) => header !== timeColumnName)
          .map((header) => ({
            header,
            score: rows.reduce((score, row) => {
              const value = String(row[header] || "").trim();
              return score + (value && extractSeconds(value) === null ? 1 : 0);
            }, 0),
          }))
          .sort((a, b) => b.score - a.score)[0]?.header || "";
      }

      function detectFallbackColumns(timeColumnName, commentColumnName) {
        const preferred = [];

        commentCandidates.forEach((keyword) => {
          headers.forEach((header) => {
            if (
              header !== timeColumnName &&
              header !== commentColumnName &&
              header.toLowerCase().includes(keyword) &&
              !preferred.includes(header)
            ) {
              preferred.push(header);
            }
          });
        });

        return preferred;
      }

      function populateSelect(select, selectedValue) {
        select.innerHTML = "";

        headers.forEach((header) => {
          const option = document.createElement("option");
          option.value = header;
          option.textContent = header;
          option.selected = header === selectedValue;
          select.append(option);
        });

        if (select.id === "commentColumn") {
          const option = document.createElement("option");
          option.value = markerDescriptionOption;
          option.textContent = "Marker Name + Description";
          option.selected = selectedValue === markerDescriptionOption;
          select.append(option);
        }
      }

      function renderPreview() {
        const previewHeaders = headers.slice(0, 6);
        const previewRows = rows.slice(0, 8);
        const thead = document.createElement("thead");
        const tbody = document.createElement("tbody");
        const headerRow = document.createElement("tr");

        if (previewHeaders.length === 0) {
          previewTable.innerHTML = "<thead><tr><th>Waiting for input</th></tr></thead><tbody><tr><td>Load or paste a CSV to preview rows.</td></tr></tbody>";
          return;
        }

        previewHeaders.forEach((header) => {
          const th = document.createElement("th");
          th.textContent = header;
          headerRow.append(th);
        });
        thead.append(headerRow);

        previewRows.forEach((row) => {
          const tr = document.createElement("tr");
          previewHeaders.forEach((header) => {
            const td = document.createElement("td");
            td.textContent = row[header] || "";
            tr.append(td);
          });
          tbody.append(tr);
        });

        previewTable.replaceChildren(thead, tbody);
      }

      function getFallbackColumnList() {
        return fallbackColumns.value
          .split(",")
          .map((column) => column.trim())
          .filter((column) => headers.includes(column));
      }

      function buildConvertedRows() {
        const timeKey = timeColumn.value;
        const commentKey = commentColumn.value;
        const fallbackList = getFallbackColumnList();
        const orderedCommentColumns = [commentKey, ...fallbackList.filter((column) => column !== commentKey)];
        const markerNameKey = headers.find((header) => (
          header !== timeKey &&
          header.trim().toLowerCase() === "marker name"
        ));
        const descriptionKey = headers.find((header) => (
          header !== timeKey &&
          header.trim().toLowerCase() === "description"
        ));
        const converted = [];
        const skipped = [];

        rows.forEach((row) => {
          const seconds = extractSeconds(row[timeKey]);
          const markerName = markerNameKey ? String(row[markerNameKey] || "").trim() : "";
          const description = descriptionKey ? String(row[descriptionKey] || "").trim() : "";
          const comment = commentKey === markerDescriptionOption
            ? [markerName || "(untitled marker)", description].filter(Boolean).join("\n")
            : orderedCommentColumns
                .map((column) => String(row[column] || "").trim())
                .find(Boolean) || "(untitled marker)";

          if (seconds === null) {
            skipped.push(row.__rowNumber);
            return;
          }

          converted.push({
            rowNumber: row.__rowNumber,
            seconds,
            comment,
          });
        });

        if (sortMode.value === "time") {
          converted.sort((a, b) => a.seconds - b.seconds || a.rowNumber - b.rowNumber);
        }

        return { converted, skipped };
      }

      function buildOutput(converted) {
        const mode = formatMode.value;

        if (mode === "srt") {
          return converted
            .map((item, index) => {
              const next = converted[index + 1];
              const end = next ? Math.max(item.seconds + 1, next.seconds) : item.seconds + 4;
              return `${index + 1}\n${formatSrtTime(item.seconds)} --> ${formatSrtTime(end)}\n${item.comment}`;
            })
            .join("\n\n");
        }

        return converted
          .map((item, index) => {
            const time = formatSeconds(item.seconds, mode === "hours" ? "hours" : "standard");
            const separator = mode === "youtube" || mode === "chapters" ? " " : " - ";
            const comment = mode === "chapters" && index === 0 && item.seconds !== 0
              ? `${item.comment} (starts at ${time})`
              : item.comment;
            return `${time}${separator}${comment}`;
          })
          .join("\n");
      }

      function updateMetrics(converted = [], skipped = []) {
        rowCount.textContent = String(rows.length);
        validCount.textContent = String(converted.length || rows.filter((row) => extractSeconds(row[timeColumn.value]) !== null).length);
        skippedCount.textContent = String(skipped.length);
      }

      function loadCsvText(text, name = "premiere-timestamps.csv") {
        const cleaned = text.replace(/^\uFEFF/, "");
        const delimiter = detectDelimiter(cleaned);
        let records = [];

        try {
          records = parseCsv(cleaned, delimiter);
        } catch (error) {
          setStatus(error.message, "error");
          return;
        }

        if (records.length === 0) {
          setStatus("Paste CSV text first, or upload your Premiere marker CSV file.", "warning");
          return;
        }

        const firstRowLooksLikeData = records[0].some((cell) => extractSeconds(cell) !== null);

        if (records.length < 2 && !firstRowLooksLikeData) {
          setStatus("Add one marker row under the header, or upload the exported CSV file.", "warning");
          return;
        }

        const normalizedRecords = firstRowLooksLikeData
          ? [
              records[0].map((_, index) => {
                if (index === 0) return "Timecode";
                if (index === 1) return "Marker Name";
                if (index === 2) return "Comment";
                return `Column ${index + 1}`;
              }),
              ...records,
            ]
          : records;

        const parsed = recordsToObjects(normalizedRecords);
        headers = parsed.headers;
        rows = parsed.rows;
        sourceName = name.replace(/\.[^.]+$/, "") || "premiere-timestamps";

        const detectedTime = detectTimeColumn();
        const detectedComment = detectCommentColumn(detectedTime);
        detectedFallbacks = detectFallbackColumns(detectedTime, detectedComment);

        populateSelect(timeColumn, detectedTime || headers[0]);
        populateSelect(commentColumn, detectedComment || headers.find((header) => header !== detectedTime) || headers[0]);
        fallbackColumns.value = detectedFallbacks.join(", ");

        convertButton.disabled = false;
        outputText = "";
        output.value = "";
        downloadButton.disabled = false;
        copyOutputButton.disabled = true;
        lineCount.textContent = "0 lines";

        const delimiterName = delimiter === "\t" ? "tab" : delimiter === ";" ? "semicolon" : "comma";
        delimiterLabel.textContent = `${delimiterName}-delimited, ${headers.length} columns`;
        dropTitle.textContent = name;
        dropMeta.textContent = `${rows.length} data rows loaded`;
        renderPreview();
        updateMetrics();
        setStatus(`Loaded ${rows.length} rows from ${name}.`);
      }

      function convertRows() {
        if (rows.length === 0) {
          setStatus("Load or paste a CSV before converting.", "error");
          return;
        }

        const { converted, skipped } = buildConvertedRows();
        outputText = buildOutput(converted);
        output.value = outputText;
        lineCount.textContent = `${converted.length} ${converted.length === 1 ? "line" : "lines"}`;
        downloadButton.disabled = converted.length === 0;
        copyOutputButton.disabled = converted.length === 0;
        updateMetrics(converted, skipped);

        if (converted.length === 0) {
          setStatus("No valid timecode rows were found.", "error");
        } else if (skipped.length > 0) {
          const listed = skipped.slice(0, 8).join(", ");
          setStatus(`Converted ${converted.length} rows. Skipped CSV rows ${listed}${skipped.length > 8 ? "..." : ""}.`, "warning");
        } else {
          setStatus(`Converted ${converted.length} rows.`);
        }
      }

      function safeFileName(name) {
        return (name || "premiere-timestamps")
          .trim()
          .replace(/[^\w.-]+/g, "-")
          .replace(/^-+|-+$/g, "") || "premiere-timestamps";
      }

      function downloadTxt() {
        if (!outputText) {
          convertRows();
        }

        if (!outputText) {
          return;
        }

        const extension = formatMode.value === "srt" ? "srt" : "txt";
        const blob = new Blob([outputText + "\n"], { type: "text/plain;charset=utf-8" });
        const link = document.createElement("a");
        link.href = URL.createObjectURL(blob);
        link.download = `${safeFileName(sourceName)}-timestamps.${extension}`;
        link.click();
        URL.revokeObjectURL(link.href);
      }

      async function copyText(text, successMessage) {
        if (!text) {
          return;
        }

        if (navigator.clipboard) {
          await navigator.clipboard.writeText(text);
        } else {
          const copyBox = document.createElement("textarea");
          copyBox.value = text;
          copyBox.style.position = "fixed";
          copyBox.style.inset = "0 auto auto 0";
          copyBox.style.opacity = "0";
          document.body.append(copyBox);
          copyBox.select();
          document.execCommand("copy");
          copyBox.remove();
        }

        setStatus(successMessage);
      }

      async function readFile(file) {
        const text = decodeTextBuffer(await file.arrayBuffer());
        rawInput.value = text;
        loadCsvText(text, file.name);
      }

      function clearAll() {
        rows = [];
        headers = [];
        outputText = "";
        sourceName = "premiere-timestamps";
        rawInput.value = "";
        output.value = "";
        timeColumn.innerHTML = "";
        commentColumn.innerHTML = "";
        fallbackColumns.value = "";
        lineCount.textContent = "0 lines";
        delimiterLabel.textContent = "No file loaded";
        dropTitle.textContent = "Choose CSV or TSV";
        dropMeta.textContent = "Drop a marker export here";
        convertButton.disabled = true;
        downloadButton.disabled = true;
        copyOutputButton.disabled = true;
        rowCount.textContent = "0";
        validCount.textContent = "0";
        skippedCount.textContent = "0";
        renderPreview();
        setStatus("Cleared.");
      }

      fileInput.addEventListener("change", () => {
        const [file] = fileInput.files;
        if (file) {
          readFile(file);
        }
      });

      ["dragenter", "dragover"].forEach((eventName) => {
        dropZone.addEventListener(eventName, (event) => {
          event.preventDefault();
          dropZone.classList.add("is-dragging");
        });
      });

      ["dragleave", "drop"].forEach((eventName) => {
        dropZone.addEventListener(eventName, (event) => {
          event.preventDefault();
          dropZone.classList.remove("is-dragging");
        });
      });

      dropZone.addEventListener("drop", (event) => {
        const [file] = event.dataTransfer.files;

        if (file) {
          readFile(file);
        }
      });

      parsePasteButton.addEventListener("click", () => loadCsvText(rawInput.value, "pasted-markers.csv"));
      convertButton.addEventListener("click", convertRows);
      downloadButton.addEventListener("click", downloadTxt);
      copyOutputButton.addEventListener("click", () => copyText(output.value, "Output copied."));
      copyInputButton.addEventListener("click", () => copyText(rawInput.value, "Input copied."));
      clearButton.addEventListener("click", clearAll);

      [timeColumn, commentColumn, formatMode, sortMode, fallbackColumns].forEach((control) => {
        control.addEventListener("change", () => {
          if (rows.length > 0) {
            convertRows();
          }
        });
      });

      sampleButton.addEventListener("click", () => {
        const sample = [
          "Timecode,Marker Name,Comment,Asset",
          "00:00:00:00,Intro,\"Cold open, use tighter music\",intro.mov",
          "00:01:12:04,Lower third,\"Add title: Alex Rivera\",interview-a.mov",
          "00:02:05:12,B-roll,\"City, skyline, morning\",broll-city.mov",
          "00:12:44:01,Final review,\"Color pass and export\",sequence.prproj",
        ].join("\n");
        rawInput.value = sample;
        loadCsvText(sample, "sample-markers.csv");
        convertRows();
      });

      document.addEventListener("keydown", (event) => {
        const command = event.ctrlKey || event.metaKey;

        if (command && event.key === "Enter") {
          event.preventDefault();
          convertRows();
        }

        if (command && event.key.toLowerCase() === "s") {
          event.preventDefault();
          downloadTxt();
        }
      });

      renderPreview();
    </script>
  </body>
</html>
