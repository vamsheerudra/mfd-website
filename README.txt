Nityasarathi website: how to maintain

Folder
  index.html          Home page
  tools.html          Tools page (one card per tool)
  style.css           Shared styles for index.html and tools.html
  script.js           Phone menu
  tools/              One .html file per tool

Add a new tool (about 5 minutes)
  1. Save the tool's HTML into the tools/ folder, for example tools/client-financial-plan.html
  2. Add the back link just after <body>:
       <div class="back-bar"><a href="../tools.html">&larr; Back to Tools</a></div>
     and copy the disclaimer block (class "tool-foot") from tools/home-loan-vs-mf.html
  3. In tools.html, copy one <div class="service"> ... </div> card, then change the number, title, description and link
  4. Commit and push to GitHub. Netlify publishes it in a minute or so.

Rules
  - Pages in the main folder link to style.css and tools.html directly.
  - Pages inside tools/ use ../ to go back up, for example ../tools.html.
  - Keep the disclaimer on every tool page. Do not promise returns.
