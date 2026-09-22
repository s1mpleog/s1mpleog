
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: var(--font-mono, monospace); }
  .root { padding: 2rem 0; }
  .hero { display: flex; align-items: center; gap: 1.5rem; margin-bottom: 2rem; }
  .avatar { width: 72px; height: 72px; border-radius: 50%; background: var(--surface-1); border: 0.5px solid var(--border-strong); display: flex; align-items: center; justify-content: center; font-size: 28px; font-weight: 500; color: var(--text-secondary); flex-shrink: 0; font-family: var(--font-mono); }
  .hero-text h1 { font-size: 22px; font-weight: 500; color: var(--text-primary); letter-spacing: -0.02em; font-family: var(--font-mono); }
  .hero-text p { font-size: 13px; color: var(--text-secondary); margin-top: 4px; font-family: var(--font-mono); }
  .badges { display: flex; gap: 6px; margin-top: 10px; flex-wrap: wrap; }
  .badge { font-size: 11px; padding: 3px 10px; border-radius: 20px; border: 0.5px solid var(--border-strong); color: var(--text-secondary); font-family: var(--font-mono); }
  .badge.cpp { border-color: #659ad2; color: #659ad2; }
  .badge.rust { border-color: #dea584; color: #dea584; }
  .badge.vk { border-color: #ac162c; color: #ac162c; }
  .section { margin-bottom: 2rem; }
  .section-label { font-size: 11px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 0.1em; margin-bottom: 0.75rem; font-family: var(--font-mono); }
  .stack-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 0; border: 0.5px solid var(--border); border-radius: 12px; overflow: hidden; }
  .stack-item { padding: 0.75rem 1rem; border-right: 0.5px solid var(--border); border-bottom: 0.5px solid var(--border); }
  .stack-item:nth-child(2n) { border-right: none; }
  .stack-item:nth-last-child(-n+2) { border-bottom: none; }
  .stack-name { font-size: 12px; font-weight: 500; color: var(--text-primary); margin-bottom: 6px; font-family: var(--font-mono); }
  .bar-wrap { display: flex; align-items: center; gap: 8px; }
  .bar-bg { flex: 1; height: 3px; background: var(--surface-1); border-radius: 2px; overflow: hidden; }
  .bar-fill { height: 100%; border-radius: 2px; }
  .bar-pct { font-size: 11px; color: var(--text-muted); min-width: 28px; text-align: right; font-family: var(--font-mono); }
  .projects-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
  .proj-card { background: var(--surface-1); border: 0.5px solid var(--border); border-radius: 12px; padding: 1rem; cursor: pointer; transition: border-color 0.15s; }
  .proj-card:hover { border-color: var(--border-strong); }
  .proj-name { font-size: 13px; font-weight: 500; color: var(--text-accent); font-family: var(--font-mono); }
  .proj-desc { font-size: 12px; color: var(--text-secondary); margin-top: 4px; line-height: 1.5; font-family: var(--font-mono); }
  .proj-tags { display: flex; gap: 4px; margin-top: 8px; flex-wrap: wrap; }
  .proj-tag { font-size: 10px; color: var(--text-muted); background: var(--surface-0); border: 0.5px solid var(--border); border-radius: 4px; padding: 2px 6px; font-family: var(--font-mono); }
  .stack-section { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
  .focus-list { background: var(--surface-1); border: 0.5px solid var(--border); border-radius: 12px; padding: 1rem; }
  .focus-list .focus-group { font-size: 11px; font-weight: 500; color: var(--text-muted); text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 6px; font-family: var(--font-mono); }
  .focus-list ul { list-style: none; }
  .focus-list ul li { font-size: 12px; color: var(--text-secondary); padding: 2px 0; font-family: var(--font-mono); }
  .focus-list ul li::before { content: "→ "; color: var(--text-muted); }
  .divider { height: 0.5px; background: var(--border); margin: 1.5rem 0; }
  .tagline { font-size: 12px; color: var(--text-muted); text-align: center; letter-spacing: 0.12em; font-family: var(--font-mono); }
</style>

<h2 class="sr-only">s1mpleog GitHub profile — systems, graphics, low-level programmer</h2>

<div class="root">
  <div class="hero">
    <div class="avatar">s1</div>
    <div class="hero-text">
      <h1>s1mpleog</h1>
      <p>systems · graphics · low-level</p>
      <div class="badges">
        <span class="badge cpp">C++23</span>
        <span class="badge rust">Rust</span>
        <span class="badge vk">Vulkan</span>
        <span class="badge">x86-64</span>
        <span class="badge">Linux</span>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">projects</div>
    <div class="projects-grid">
      <div class="proj-card" onclick="openLink('https://github.com/s1mpleog/wind')">
        <div class="proj-name">wind</div>
        <div class="proj-desc">Vulkan renderer and graphics engine built from scratch.</div>
        <div class="proj-tags"><span class="proj-tag">C++</span><span class="proj-tag">Vulkan</span><span class="proj-tag">Graphics</span></div>
      </div>
      <div class="proj-card" onclick="openLink('https://github.com/s1mpleog/wind-cooker')">
        <div class="proj-name">wind-cooker</div>
        <div class="proj-desc">Asset pipeline and content cooker for Wind.</div>
        <div class="proj-tags"><span class="proj-tag">Rust</span><span class="proj-tag">Tooling</span></div>
      </div>
      <div class="proj-card" onclick="openLink('https://github.com/s1mpleog/peel')">
        <div class="proj-name">peel</div>
        <div class="proj-desc">PE file visualizer for inspecting Windows executables.</div>
        <div class="proj-tags"><span class="proj-tag">C++</span><span class="proj-tag">PE</span><span class="proj-tag">Windows</span></div>
      </div>
      <div class="proj-card" onclick="openLink('https://github.com/s1mpleog/clmm-math')">
        <div class="proj-name">clmm-math</div>
        <div class="proj-desc">Rust math library for Solana CLMM protocol work.</div>
        <div class="proj-tags"><span class="proj-tag">Rust</span><span class="proj-tag">DeFi</span></div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">stack</div>
    <div class="stack-grid">
      <div class="stack-item">
        <div class="stack-name">C / C++23</div>
        <div class="bar-wrap">
          <div class="bar-bg"><div class="bar-fill" style="width:100%; background:#659ad2;"></div></div>
          <span class="bar-pct">100%</span>
        </div>
      </div>
      <div class="stack-item">
        <div class="stack-name">Rust</div>
        <div class="bar-wrap">
          <div class="bar-bg"><div class="bar-fill" style="width:75%; background:#dea584;"></div></div>
          <span class="bar-pct">75%</span>
        </div>
      </div>
      <div class="stack-item">
        <div class="stack-name">Vulkan</div>
        <div class="bar-wrap">
          <div class="bar-bg"><div class="bar-fill" style="width:75%; background:#ac162c;"></div></div>
          <span class="bar-pct">75%</span>
        </div>
      </div>
      <div class="stack-item">
        <div class="stack-name">x86 ASM</div>
        <div class="bar-wrap">
          <div class="bar-bg"><div class="bar-fill" style="width:60%; background: var(--text-muted);"></div></div>
          <span class="bar-pct">60%</span>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">currently exploring</div>
    <div class="stack-section">
      <div class="focus-list">
        <div class="focus-group">systems</div>
        <ul>
          <li>allocators</li>
          <li>memory models</li>
          <li>ABI & calling conventions</li>
          <li>compiler internals</li>
          <li>operating systems</li>
        </ul>
      </div>
      <div class="focus-list">
        <div class="focus-group">graphics</div>
        <ul>
          <li>Vulkan</li>
          <li>GPU architecture</li>
          <li>rendering techniques</li>
          <li>shader authoring</li>
          <li>asset pipelines</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="divider"></div>
  <div class="tagline">build · break · understand · repeat</div>
</div>
