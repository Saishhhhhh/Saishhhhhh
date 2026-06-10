<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body { font-family: 'Segoe UI', system-ui, sans-serif; }
  .readme-root { background: #0d0d14; color: #e5eef8; font-family: 'Segoe UI', system-ui, sans-serif; padding: 0; min-height: 100vh; line-height: 1.6; }
  .hero { background: #0d0d14; padding: 2.5rem 2rem 1.5rem; border-bottom: 1px solid #1e1e30; position: relative; overflow: hidden; }
  .hero::before, .hero::after { content: ''; position: absolute; border-radius: 999px; filter: blur(6px); pointer-events: none; }
  .hero::before { top: -70px; right: -70px; width: 280px; height: 280px; background: radial-gradient(circle, rgba(124,58,237,0.18) 0%, transparent 70%); }
  .hero::after { bottom: -50px; left: 25%; width: 200px; height: 200px; background: radial-gradient(circle, rgba(6,182,212,0.10) 0%, transparent 70%); }
  .terminal-window { background: #13131f; border: 1px solid #2a2a40; border-radius: 10px; overflow: hidden; max-width: 680px; font-family: 'JetBrains Mono', 'Fira Code', 'Courier New', monospace; box-shadow: 0 10px 30px rgba(0, 0, 0, 0.25); }
  .terminal-bar { background: #1a1a2e; padding: 10px 14px; display: flex; align-items: center; gap: 6px; border-bottom: 1px solid #2a2a40; }
  .dot { width: 11px; height: 11px; border-radius: 50%; }
  .dot.red { background: #ff5f57; }
  .dot.yellow { background: #ffbd2e; }
  .dot.green { background: #28c840; }
  .terminal-title { font-size: 11px; color: #6b7280; margin-left: auto; font-family: var(--font-mono); }
  .terminal-body { padding: 1.25rem 1.5rem; font-size: 13px; line-height: 1.9; }
  .prompt { color: #8b5cf6; }
  .cmd { color: #e5eef8; }
  .out-key { color: #22d3ee; }
  .out-str { color: #86efac; }
  .out-arr { color: #fbbf24; }
  .cursor { display: inline-block; width: 8px; height: 14px; background: #8b5cf6; vertical-align: middle; animation: blink 1.1s step-end infinite; }
  @keyframes blink { 0%, 100% { opacity: 1; } 50% { opacity: 0; } }
  .socials-bar { padding: 1.25rem 2rem; display: flex; gap: 10px; flex-wrap: wrap; align-items: center; border-bottom: 1px solid #1e1e30; }
  .badge { display: inline-flex; align-items: center; gap: 7px; padding: 6px 13px; border-radius: 6px; font-size: 12px; font-weight: 500; text-decoration: none; border: 1px solid; cursor: pointer; transition: opacity 0.15s; }
  .badge:hover { opacity: 0.75; }
  .badge-li { background: #00335e; border-color: #0a66c2; color: #60a5fa; }
  .badge-port { background: #1a1020; border-color: #7c3aed; color: #c4b5fd; }
  .badge-mail { background: #1f1000; border-color: #ea4335; color: #fca5a5; }
  .badge-disc { background: #0e0e2a; border-color: #5865f2; color: #a5b4fc; }
  .section { padding: 2rem 2rem; border-bottom: 1px solid #1e1e30; }
  .section-label { font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; color: #6b7280; font-family: monospace; margin-bottom: 1rem; }
  .section-label span { color: #8b5cf6; }
  .stack-group { margin-bottom: 1.5rem; }
  .stack-group-title { font-size: 11px; color: #94a3b8; font-family: monospace; letter-spacing: 0.1em; margin-bottom: 10px; padding-left: 2px; }
  .stack-group-title::before { content: '// '; color: #475569; }
  .icon-grid { display: flex; flex-wrap: wrap; gap: 8px; }
  .stack-chip { background: #13131f; border: 1px solid #2a2a40; border-radius: 6px; padding: 5px 10px; font-size: 12px; color: #cbd5e1; font-family: monospace; white-space: nowrap; display: flex; align-items: center; gap: 6px; }
  .chip-dot { width: 6px; height: 6px; border-radius: 50%; flex-shrink: 0; }
  .dot-violet { background: #8b5cf6; }
  .dot-cyan { background: #22d3ee; }
  .dot-orange { background: #fb923c; }
  .dot-green { background: #4ade80; }
  .dot-blue { background: #60a5fa; }
  .dot-pink { background: #f472b6; }
  .dot-yellow { background: #facc15; }
  .dot-gray { background: #94a3b8; }
  .stats-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
  .stat-card { background: #13131f; border: 1px solid #2a2a40; border-radius: 10px; padding: 1rem; }
  .stat-note { font-size: 11px; color: #94a3b8; font-family: monospace; margin-top: 10px; }
  .small-note { font-size: 11px; color: #64748b; font-family: monospace; }
  .footer { padding: 1.5rem 2rem; text-align: center; font-size: 11px; color: #94a3b8; font-family: monospace; }
  .footer-quote { font-style: italic; color: #cbd5e1; margin-bottom: 6px; }
</style>

<div class="readme-root">
  <div class="hero">
    <div class="terminal-window">
      <div class="terminal-bar">
        <div class="dot red"></div>
        <div class="dot yellow"></div>
        <div class="dot green"></div>
        <span class="terminal-title">saish@github ~ whoami</span>
      </div>
      <div class="terminal-body">
        <div><span class="prompt">❯ </span><span class="cmd">cat profile.json</span></div>
        <div style="margin-top:8px; padding-left: 4px;">
          {<br>
          &nbsp;&nbsp;<span class="out-key">"name"</span>: <span class="out-str">"Saish Baviskar"</span>,<br>
          &nbsp;&nbsp;<span class="out-key">"role"</span>: <span class="out-arr">["AI Engineer", "ML Engineer", "Data Scientist"]</span>,<br>
          &nbsp;&nbsp;<span class="out-key">"currently"</span>: <span class="out-str">"Cantilever Labs · AI Intern"</span>,<br>
          &nbsp;&nbsp;<span class="out-key">"location"</span>: <span class="out-str">"Pune, India 🇮🇳"</span>,<br>
          &nbsp;&nbsp;<span class="out-key">"focus"</span>: <span class="out-arr">["Agentic AI", "RAG Systems", "LLM Pipelines"]</span>,<br>
          &nbsp;&nbsp;<span class="out-key">"motto"</span>: <span class="out-str">"Making projects to solve my own problems"</span><br>
          }<br>
        </div>
        <div style="margin-top:8px;"><span class="prompt">❯ </span><span class="cursor"></span></div>
      </div>
    </div>
  </div>

  <div class="socials-bar">
    <a class="badge badge-li" href="https://www.linkedin.com/in/saishhhhhh/" target="_blank">🔗 LinkedIn</a>
    <a class="badge badge-port" href="https://saishhhhhh.vercel.app/" target="_blank">⬡ Portfolio</a>
    <a class="badge badge-mail" href="mailto:bsaish404@gmail.com">✉ Gmail</a>
    <a class="badge badge-disc" href="https://discord.com/users/saish4593" target="_blank">◈ Discord</a>
  </div>

  <div class="section">
    <div class="section-label"><span>01</span> / tech stack</div>
    <div class="stack-group">
      <div class="stack-group-title">AI &amp; LLM Systems</div>
      <div class="icon-grid">
        <span class="stack-chip"><span class="chip-dot dot-violet"></span>LangChain</span>
        <span class="stack-chip"><span class="chip-dot dot-violet"></span>LangGraph</span>
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>RAG</span>
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>Agentic AI</span>
        <span class="stack-chip"><span class="chip-dot dot-pink"></span>MCP</span>
        <span class="stack-chip"><span class="chip-dot dot-pink"></span>Prompt Eng.</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-title">ML / DL</div>
      <div class="icon-grid">
        <span class="stack-chip"><span class="chip-dot dot-orange"></span>PyTorch</span>
        <span class="stack-chip"><span class="chip-dot dot-orange"></span>TensorFlow</span>
        <span class="stack-chip"><span class="chip-dot dot-orange"></span>Keras</span>
        <span class="stack-chip"><span class="chip-dot dot-yellow"></span>HuggingFace</span>
        <span class="stack-chip"><span class="chip-dot dot-yellow"></span>SBERT</span>
        <span class="stack-chip"><span class="chip-dot dot-yellow"></span>Transformers</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-title">Languages</div>
      <div class="icon-grid">
        <span class="stack-chip"><span class="chip-dot dot-blue"></span>Python</span>
        <span class="stack-chip"><span class="chip-dot dot-yellow"></span>JavaScript</span>
        <span class="stack-chip"><span class="chip-dot dot-blue"></span>SQL</span>
        <span class="stack-chip"><span class="chip-dot dot-gray"></span>C / C++</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-title">Databases &amp; Vector Stores</div>
      <div class="icon-grid">
        <span class="stack-chip"><span class="chip-dot dot-green"></span>Pinecone</span>
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>Qdrant</span>
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>ChromaDB</span>
        <span class="stack-chip"><span class="chip-dot dot-green"></span>MongoDB</span>
        <span class="stack-chip"><span class="chip-dot dot-blue"></span>PostgreSQL</span>
        <span class="stack-chip"><span class="chip-dot dot-blue"></span>MySQL</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-group-title">Web &amp; Backend</div>
      <div class="icon-grid">
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>React</span>
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>FastAPI</span>
        <span class="stack-chip"><span class="chip-dot dot-green"></span>Node.js</span>
        <span class="stack-chip"><span class="chip-dot dot-gray"></span>Express</span>
        <span class="stack-chip"><span class="chip-dot dot-blue"></span>Redux</span>
        <span class="stack-chip"><span class="chip-dot dot-cyan"></span>Tailwind</span>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label"><span>02</span> / github activity</div>
    <div class="stats-row">
      <div class="stat-card">
        <img src="https://github-readme-stats.vercel.app/api?username=saishhhhhh&show_icons=true&theme=tokyo-night&hide_border=true" alt="GitHub stats" style="width:100%; border-radius:8px;" />
      </div>
      <div class="stat-card">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=saishhhhhh&theme=tokyo-night&hide_border=true" alt="GitHub streak" style="width:100%; border-radius:8px;" />
      </div>
    </div>
    <div class="stat-note">Commit history, contribution streak, and daily coding rhythm from your GitHub profile.</div>
  </div>

  <div class="section">
    <div class="section-label"><span>03</span> / contributions</div>
    <div class="small-note">GitHub contribution snake and activity are ready to render in your profile repository.</div>
  </div>

  <div class="footer">
    <div class="footer-quote">"Making projects to solve my own problems"</div>
    <div>⭐ if you like what you see, drop a star · let's build something</div>
  </div>
</div>
