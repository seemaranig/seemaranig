
<style>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'DM Sans',sans-serif}
.wrap{max-width:860px;margin:0 auto;padding:2rem 1.5rem;color:var(--color-text-primary)}
.hero{display:grid;grid-template-columns:1fr auto;gap:2rem;align-items:center;padding:2.5rem 0 2rem}
.hero-left{}
.eyebrow{font-family:'Space Mono',monospace;font-size:11px;letter-spacing:0.15em;color:var(--color-text-secondary);text-transform:uppercase;margin-bottom:.75rem}
.name{font-size:2.6rem;font-weight:300;line-height:1.15;letter-spacing:-0.02em;margin-bottom:.5rem}
.name span{font-weight:500}
.tagline{font-size:1rem;color:var(--color-text-secondary);font-weight:300;line-height:1.6;max-width:480px}
.avatar-ring{width:120px;height:120px;border-radius:50%;background:linear-gradient(135deg,#0F6E56 0%,#5DCAA5 50%,#1D9E75 100%);padding:3px;flex-shrink:0}
.avatar-inner{width:100%;height:100%;border-radius:50%;background:var(--color-background-primary);display:flex;align-items:center;justify-content:center;font-family:'Space Mono',monospace;font-size:1.4rem;font-weight:700;color:#0F6E56}
.divider{height:0.5px;background:var(--color-border-tertiary);margin:0 0 2rem}
.grid3{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:var(--color-border-tertiary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);overflow:hidden;margin-bottom:2rem}
.stat-block{background:var(--color-background-primary);padding:1.25rem 1rem;text-align:center}
.stat-val{font-family:'Space Mono',monospace;font-size:1.5rem;font-weight:700;color:var(--color-text-primary)}
.stat-lbl{font-size:11px;letter-spacing:0.1em;text-transform:uppercase;color:var(--color-text-secondary);margin-top:4px}
.section-label{font-family:'Space Mono',monospace;font-size:10px;letter-spacing:0.18em;text-transform:uppercase;color:var(--color-text-tertiary);margin-bottom:1rem;display:flex;align-items:center;gap:8px}
.section-label::after{content:'';flex:1;height:0.5px;background:var(--color-border-tertiary)}
.currently{background:var(--color-background-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;margin-bottom:2rem}
.now-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:.75rem;margin-top:1rem}
.now-item{display:flex;align-items:flex-start;gap:10px;font-size:14px;color:var(--color-text-secondary);line-height:1.5}
.dot{width:6px;height:6px;border-radius:50%;background:#1D9E75;flex-shrink:0;margin-top:6px}
.now-item strong{color:var(--color-text-primary);font-weight:500}
.stack{margin-bottom:2rem}
.pills{display:flex;flex-wrap:wrap;gap:6px;margin-top:.75rem}
.pill{font-family:'Space Mono',monospace;font-size:11px;padding:4px 10px;border-radius:4px;border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);background:var(--color-background-primary)}
.pill.accent{border-color:#0F6E56;color:#0F6E56;background:#E1F5EE}
.projects{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-bottom:2rem}
.proj-card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.25rem;transition:border-color .2s}
.proj-card:hover{border-color:var(--color-border-secondary)}
.proj-icon{font-size:22px;margin-bottom:.75rem}
.proj-title{font-size:14px;font-weight:500;margin-bottom:.35rem}
.proj-desc{font-size:12px;color:var(--color-text-secondary);line-height:1.5}
.proj-tags{display:flex;flex-wrap:wrap;gap:4px;margin-top:.75rem}
.proj-tag{font-size:10px;font-family:'Space Mono',monospace;padding:2px 7px;border-radius:3px;background:var(--color-background-secondary);color:var(--color-text-tertiary)}
.awards{display:flex;gap:12px;margin-bottom:2rem}
.award{flex:1;background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:1rem;text-align:center}
.award-icon{font-size:1.5rem;margin-bottom:.4rem}
.award-name{font-size:12px;font-weight:500}
.award-sub{font-size:11px;color:var(--color-text-secondary);margin-top:2px}
.connect{display:flex;align-items:center;gap:1rem;flex-wrap:wrap}
.connect-link{display:flex;align-items:center;gap:6px;font-size:13px;font-family:'Space Mono',monospace;color:var(--color-text-secondary);text-decoration:none;border:0.5px solid var(--color-border-secondary);padding:8px 14px;border-radius:var(--border-radius-md)}
.connect-link:hover{color:var(--color-text-primary);border-color:var(--color-border-primary)}
.connect-link i{font-size:16px}
.footer{margin-top:2rem;padding-top:1.5rem;border-top:0.5px solid var(--color-border-tertiary);font-family:'Space Mono',monospace;font-size:11px;color:var(--color-text-tertiary);text-align:center;letter-spacing:0.05em}
.badge-bar{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:2rem}
.badge{font-family:'Space Mono',monospace;font-size:10px;padding:4px 10px;border-radius:20px;letter-spacing:0.05em}
.b-green{background:#E1F5EE;color:#0F6E56}
.b-blue{background:#E6F1FB;color:#185FA5}
.b-amber{background:#FAEEDA;color:#854F0B}
.b-purple{background:#EEEDFE;color:#534AB7}
@media(prefers-color-scheme:dark){
.b-green{background:#085041;color:#9FE1CB}
.b-blue{background:#0C447C;color:#B5D4F4}
.b-amber{background:#633806;color:#FAC775}
.b-purple{background:#3C3489;color:#CECBF6}
.pill.accent{background:#085041;color:#9FE1CB;border-color:#085041}
.avatar-inner{background:var(--color-background-primary);color:#5DCAA5}
}
</style>
<div class="wrap">
  <h2 class="sr-only" style="position:absolute;width:1px;height:1px;overflow:hidden">GitHub profile preview for Seemarani G — Generative AI Engineer</h2>

  <div class="hero">
    <div class="hero-left">
      <p class="eyebrow">Chennai, India · Open to opportunities</p>
      <h1 class="name">Hi, I'm <span>Seemarani G</span> 👋</h1>
      <p class="tagline">Building enterprise AI that sees, listens, and speaks — RAG systems, conversational agents, voice AI, and digital humans with Unity & Unreal Engine.</p>
    </div>
    <div class="avatar-ring">
      <div class="avatar-inner">SG</div>
    </div>
  </div>

  <div class="badge-bar">
    <span class="badge b-green">Generative AI Engineer</span>
    <span class="badge b-blue">Conversational AI</span>
    <span class="badge b-amber">Voice AI</span>
    <span class="badge b-purple">Digital Humans</span>
  </div>

  <div class="divider"></div>

  <div class="grid3">
    <div class="stat-block">
      <div class="stat-val">6+</div>
      <div class="stat-lbl">Featured projects</div>
    </div>
    <div class="stat-block">
      <div class="stat-val">2×</div>
      <div class="stat-lbl">Award winner</div>
    </div>
    <div class="stat-block">
      <div class="stat-val">RAG</div>
      <div class="stat-lbl">Specialization</div>
    </div>
  </div>

  <div class="currently">
    <p class="section-label">Currently working on</p>
    <div class="now-grid">
      <div class="now-item"><span class="dot"></span><div>Enterprise <strong>RAG & Conversational AI</strong> solutions</div></div>
      <div class="now-item"><span class="dot"></span><div><strong>LLMs, AI Agents</strong> & Autonomous systems</div></div>
      <div class="now-item"><span class="dot"></span><div><strong>Voice AI</strong> — STT, TTS & AI Avatars</div></div>
      <div class="now-item"><span class="dot"></span><div>AI integration with <strong>Unity & Unreal Engine</strong></div></div>
    </div>
  </div>

  <div class="stack">
    <p class="section-label">Tech stack</p>
    <div class="pills">
      <span class="pill accent">Azure OpenAI</span>
      <span class="pill accent">LangChain</span>
      <span class="pill accent">CrewAI</span>
      <span class="pill accent">FAISS</span>
      <span class="pill">Python</span>
      <span class="pill">FastAPI</span>
      <span class="pill">Docker</span>
      <span class="pill">Azure</span>
      <span class="pill">AWS</span>
      <span class="pill">AKS</span>
      <span class="pill">Azure Speech</span>
      <span class="pill">Unity</span>
      <span class="pill">Unreal Engine</span>
      <span class="pill">MetaHuman</span>
      <span class="pill">RAG</span>
      <span class="pill">Prompt Engineering</span>
      <span class="pill">CI/CD</span>
      <span class="pill">GitHub Actions</span>
    </div>
  </div>

  <div class="projects">
    <p class="section-label" style="grid-column:1/-1">Featured projects</p>
    <div class="proj-card">
      <div class="proj-icon">🧠</div>
      <div class="proj-title">Enterprise RAG Platform</div>
      <div class="proj-desc">AI-powered enterprise search with Azure OpenAI, LangChain & FAISS. Production-grade, scalable retrieval pipeline.</div>
      <div class="proj-tags"><span class="proj-tag">Azure OpenAI</span><span class="proj-tag">LangChain</span><span class="proj-tag">FAISS</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-icon">🎙️</div>
      <div class="proj-title">Voice AI Assistant</div>
      <div class="proj-desc">Real-time speech conversation agent with low-latency STT→LLM→TTS pipeline for enterprise deployments.</div>
      <div class="proj-tags"><span class="proj-tag">Azure Speech</span><span class="proj-tag">Python</span><span class="proj-tag">FastAPI</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-icon">🤖</div>
      <div class="proj-title">Multi-Agent AI System</div>
      <div class="proj-desc">Autonomous AI agents built with CrewAI for complex orchestration and multi-step enterprise workflows.</div>
      <div class="proj-tags"><span class="proj-tag">CrewAI</span><span class="proj-tag">LangChain</span><span class="proj-tag">Azure</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-icon">🎭</div>
      <div class="proj-title">Unreal MetaHuman Assistant</div>
      <div class="proj-desc">Digital human powered by LLMs and Voice AI — can see, listen, and speak in real time inside Unreal Engine.</div>
      <div class="proj-tags"><span class="proj-tag">Unreal Engine</span><span class="proj-tag">MetaHuman</span><span class="proj-tag">Voice AI</span></div>
    </div>
  </div>

  <p class="section-label">Achievements</p>
  <div class="awards">
    <div class="award">
      <div class="award-icon">🥇</div>
      <div class="award-name">Circle Champion</div>
      <div class="award-sub">Top performer award</div>
    </div>
    <div class="award">
      <div class="award-icon">🌟</div>
      <div class="award-name">Rookie Star</div>
      <div class="award-sub">Early excellence award</div>
    </div>
    <div class="award">
      <div class="award-icon">🚀</div>
      <div class="award-name">Enterprise AI</div>
      <div class="award-sub">Digital human delivery</div>
    </div>
    <div class="award">
      <div class="award-icon">🎯</div>
      <div class="award-name">Production-grade</div>
      <div class="award-sub">Conversational AI systems</div>
    </div>
  </div>

  <p class="section-label">Connect</p>
  <div class="connect">
    <a class="connect-link" href="https://www.linkedin.com/in/seemarani-g/"><i class="ti ti-brand-linkedin" aria-hidden="true"></i> LinkedIn</a>
    <a class="connect-link" href="mailto:seemarani2599@gmail.com"><i class="ti ti-mail" aria-hidden="true"></i> seemarani2599@gmail.com</a>
    <a class="connect-link" href="#"><i class="ti ti-file-text" aria-hidden="true"></i> Resume PDF</a>
  </div>

  <div class="footer">⚡ building AI-powered MetaHumans that can see, listen and talk</div>
</div>
