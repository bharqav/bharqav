<!-- ================================================================= -->
<!-- 1. CYBERPUNK SYSTEMS HEADER BANNER                                -->
<!-- ================================================================= -->

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0d1117&height=220&section=header&text=Bhargav&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Systems%20%E2%80%A2%20Baremetal%20AI%20%E2%80%A2%20Distributed%20Infra&descFontSize=20&descColor=38bdf8&descAlignY=62&descAlign=50" width="100%" alt="Header Banner" />
</div>

<div align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&duration=2800&pause=1000&color=38BDF8&center=true&vCenter=true&multiline=false&width=650&height=40&lines=Building+baremetal+LLM+inference+engines+in+C99;Contributing+to+Microsoft+OpenVMM+%26+OCI+Container+Runtimes;Designing+Raft-consensus+distributed+key-value+stores;Executing+fused+integer+GEMV+on+AVX-512+and+NEON" alt="Typing SVG" />
  </a>
</div>

<div align="center">
  <p>
    <code>⚡ [STATUS: ONLINE] // Core: Linux x86_64 // Dialect: C99 / Rust / C++20 // Mode: Maximum Mechanical Sympathy</code>
  </p>
</div>

<br/>

<!-- ================================================================= -->
<!-- 2. CONTRIBUTION SNAKE GAME (3D ANIMATED)                          -->
<!-- ================================================================= -->

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/bharqav/bharqav/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/bharqav/bharqav/output/github-contribution-grid-snake.svg">
    <img alt="GitHub Contribution Snake Animation" src="https://raw.githubusercontent.com/bharqav/bharqav/output/github-contribution-grid-snake-dark.svg" width="100%" />
  </picture>
</div>

<br/>

<!-- ================================================================= -->
<!-- 3. GLASSPHORE TERMINAL INTERACTIVE HUD                            -->
<!-- ================================================================= -->

<div align="center">
  <table>
    <tr>
      <td width="850" style="background-color: #0d1117; border: 1px solid #1e293b; border-radius: 8px;">
        <div style="padding: 8px 12px; border-bottom: 1px solid #1e293b; font-family: monospace; font-size: 13px; color: #94a3b8;">
          🔴 &nbsp; 🟡 &nbsp; 🟢 &nbsp; &nbsp; <b>bharqav@workstation: ~ (x86_64 / baremetal)</b>
        </div>
      </td>
    </tr>
  </table>
</div>

```c
/**
 * @file sysinfo.c
 * @brief Host developer runtime identity and system configuration.
 */

#include <stdio.h>
#include <stdint.h>

typedef struct {
    const char *name;
    const char *role;
    const char *core_focus[4];
    const char *current_kernel;
    uint32_t   favorite_flags;
} dev_t;

int main(void) {
    const dev_t me = {
        .name           = "Bhargav",
        .role           = "Systems and AI Infrastructure Engineer",
        .core_focus     = {
            "Quantized LLM Runtimes (C99)",
            "Hypervisor Virtualization (VirtIO / OpenVMM)",
            "Container Runtimes (OCI / Cgroups v2)",
            "Distributed Consensus (Raft / WAL)"
        },
        .current_kernel = "Fused Integer GEMV on AVX2 / AVX-512 VNNI",
        .favorite_flags = (1 << 3) /* -O3 -march=native -fopenmp -Wall -Wextra */
    };

    printf("[%s] %s\n", me.name, me.role);
    return 0;
}
```

<br/>

<!-- ================================================================= -->
<!-- 4. GITHUB TROPHIES / ACHIEVEMENTS GRID                            -->
<!-- ================================================================= -->

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=bharqav&theme=onedark&no-frame=true&margin-w=15&row=1&column=6" width="100%" alt="GitHub Trophies" />
</div>

<br/>

<!-- ================================================================= -->
<!-- 5. OPEN SOURCE CONTRIBUTIONS CASE STUDIES                         -->
<!-- ================================================================= -->

### 🌐 Open Source Contributions

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🛡️ <a href="https://github.com/crucible-security/crucible">Crucible Security</a>: Tool Injection Assessment Module</h4>
      <p><code>PR #64</code> (Issue #49) | <b>AI Red-Teaming & Security</b></p>
      <ul>
        <li>Built an adversarial attack engine covering <b>OWASP AGENT-004 (Tool Misuse)</b> across MCP and tool-augmented agents.</li>
        <li>Implemented 4 attack classes and 20 adversarial vectors simulating privilege escalation, prompt-to-tool manipulation, and system prompt override attacks across <b>286+ passing tests</b>.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Security-OWASP%20AGENT--004-red?style=flat-square" />
        <img src="https://img.shields.io/badge/Agentic%20AI-MCP%20Trust%20Boundary-blueviolet?style=flat-square" />
        <img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h4>🚦 <a href="https://github.com/crucible-security/crucible">Crucible Security</a>: CI/CD Security Gating</h4>
      <p><code>PR #64</code> (Issue #52) | <b>Pipeline Policy Enforcement</b></p>
      <ul>
        <li>Engineered a <code>--fail-on</code> severity threshold CLI flag to block deployment pipelines when scan findings meet or exceed target severity (HIGH, CRITICAL).</li>
        <li>Authored reusable GitHub Actions workflow templates for automated agent vulnerability scanning, artifact reporting, and policy gating.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/CI%2FCD-Security%20Gating-red?style=flat-square" />
        <img src="https://img.shields.io/badge/GitHub%20Actions-Workflow%20Automation-blue?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>🖥️ <a href="https://github.com/microsoft/openvmm">Microsoft OpenVMM</a>: VirtIO Spurious Interrupt Fix</h4>
      <p><code>PR #4226</code> | <b>Virtualization Transport Core</b></p>
      <ul>
        <li>Fixed a spurious configuration-change interrupt emitted during the <code>DRIVER_OK</code> state transition by establishing that driver activation does not alter device configuration layout.</li>
        <li>Audited <code>INTx/MSI-X</code> and MMIO interrupt signaling paths across transports, ensuring <code>config_generation</code> strictly increments only during <code>FEATURES_OK</code> negotiation.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Virtualization-VirtIO%20Core-0078D4?style=flat-square" />
        <img src="https://img.shields.io/badge/Rust-Systems%20Kernel-DEA584?style=flat-square&logo=rust&logoColor=white" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h4>📦 <a href="https://github.com/youki-dev/youki">youki</a>: OCI Live Memory & Cgroups v2 Controller</h4>
      <p><code>PR #3688</code> | <b>OCI Container Runtime</b></p>
      <ul>
        <li>Piped <code>--memory</code>, <code>--memory-reservation</code>, and <code>--memory-swap</code> in <code>youki update</code> through <code>LinuxMemoryBuilder</code> into the kernel cgroup controller layer.</li>
        <li>Corrected CLI types to signed <code>Option&lt;i64&gt;</code> to safely represent <code>-1</code> unlimited allocations, adding regression integration tests for <code>memory.max</code> and <code>memory.swap.max</code>.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Containers-OCI%20Runtime-orange?style=flat-square" />
        <img src="https://img.shields.io/badge/Linux%20Kernel-Cgroups%20v2-333333?style=flat-square&logo=linux&logoColor=white" />
      </p>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- 6. FEATURED SYSTEMS ARCHITECTURE SHOWCASE                         -->
<!-- ================================================================= -->

### 🛠️ Featured Systems

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">⚡ <a href="https://github.com/bharqav/quantr-in-c">quantr-in-c</a></h3>
      <p><b>Zero-dependency quantized LLM and MoE inference runtime in portable C99.</b></p>
      <ul>
        <li><b>Fused SIMD GEMV</b>: Direct <code>_mm256_maddubs_epi16</code> and <code>_mm512_dpbusd_epi32</code> integer dot-products with zero dynamic allocations on hot path.</li>
        <li><b>Rigorous Verification</b>: 15 bit-exact mathematical test gates covering quantization, RoPE, RMSNorm, and cross-backend parity.</li>
        <li><b>Sub-200MB Floor</b>: Paged Q8_0 KV cache and zero-copy mmap execution for 30B MoE models on DRAM-constrained machines.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/C99-00599C?style=flat-square&logo=c&logoColor=white" />
        <img src="https://img.shields.io/badge/SIMD-AVX2%20%2F%20AVX512-orange?style=flat-square" />
        <img src="https://img.shields.io/badge/Inference-GGUF-green?style=flat-square" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">🐚 <a href="https://github.com/bharqav/mysh">mysh</a></h3>
      <p><b>Production-grade POSIX mini-shell implemented in C++.</b></p>
      <ul>
        <li><b>Recursive AST Parser</b>: Full support for multi-stage pipelines (<code>|</code>), subshells, file descriptor redirections, and background operators.</li>
        <li><b>Job Control Subsystem</b>: Robust foreground and background process group signaling, terminal control, and stopped job management.</li>
        <li><b>Path & Alias Resolution</b>: Native directory stack, alias substitution, and wildcard expansion.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/C%2B%2B20-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
        <img src="https://img.shields.io/badge/POSIX-Unix%20Signals-red?style=flat-square" />
        <img src="https://img.shields.io/badge/Process-Job%20Control-blue?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">📦 <a href="https://github.com/bharqav/distributed-kv-store">distributed-kv-store</a></h3>
      <p><b>Fault-tolerant distributed key-value store built from first principles.</b></p>
      <ul>
        <li><b>Raft Consensus</b>: Complete leader election, log replication, snapshotting, and cluster membership reconfiguration.</li>
        <li><b>Consistent Hashing</b>: Dynamic node ring with virtual tokens for balanced data distribution and minimal partition rebalancing.</li>
        <li><b>Storage Primitives</b>: Hybrid Logical Clocks (HLC) for causal consistency with append-only Write-Ahead Logging (WAL).</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Consensus-Raft%20Protocol-blueviolet?style=flat-square" />
        <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
        <img src="https://img.shields.io/badge/Storage-WAL%20Engine-teal?style=flat-square" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">🔍 <a href="https://github.com/bharqav/ultimate-hybrid-rag">ultimate-hybrid-rag</a></h3>
      <p><b>High-throughput hybrid vector and lexical retrieval engine.</b></p>
      <ul>
        <li><b>Reciprocal Rank Fusion</b>: Blends dense neural vector embeddings with BM25 sparse lexical inverted indexes.</li>
        <li><b>Cross-Encoder Neural Reranking</b>: Two-stage retrieval pipeline with dynamic score normalization.</li>
        <li><b>Sub-10ms Latency</b>: Concurrent semantic chunking and zero-copy vector scoring.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white" />
        <img src="https://img.shields.io/badge/Retrieval-Vector%20%2B%20BM25-blue?style=flat-square" />
        <img src="https://img.shields.io/badge/Embeddings-Transformers-yellow?style=flat-square" />
      </p>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- 7. CORE TECHNICAL ARSENAL                                         -->
<!-- ================================================================= -->

### ⚙️ Core Technical Arsenal

<table width="100%">
  <tr>
    <td width="25%" valign="top">
      <b>Languages</b><br/>
      <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=c,cpp,rust,go,python,ts" alt="Languages" /></a>
    </td>
    <td width="25%" valign="top">
      <b>Systems & Compute</b><br/>
      <img src="https://img.shields.io/badge/SIMD-AVX2%20%2F%20AVX512-0284c7?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/ARM-NEON%20Intrinsics-0284c7?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/Concurrency-OpenMP%20%2F%20pthreads-0284c7?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/Memory-mmap%20%2F%20Zero--Alloc-0284c7?style=flat-square" />
    </td>
    <td width="25%" valign="top">
      <b>Infra & Storage</b><br/>
      <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=docker,linux,postgres,redis,git" alt="Infrastructure" /></a>
    </td>
    <td width="25%" valign="top">
      <b>Toolchain & Build</b><br/>
      <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=cmake,githubactions,bash,vscode" alt="Toolchain" /></a>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- 8. ENGINEERING TELEMETRY & METRICS                                -->
<!-- ================================================================= -->

### 📊 Engineering Metrics

<div align="center">
  <table border="0">
    <tr>
      <td>
        <img src="https://github-readme-stats.vercel.app/api?username=bharqav&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true&bg_color=0d1117&title_color=38bdf8&icon_color=38bdf8&text_color=94a3b8" width="410" alt="GitHub Stats" />
      </td>
      <td>
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=bharqav&theme=tokyonight&hide_border=true&background=0d1117&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8&sideLabels=94a3b8&dates=64748b" width="380" alt="GitHub Streak" />
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bharqav&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=38bdf8&text_color=94a3b8&langs_count=8" width="500" alt="Top Languages" />
      </td>
    </tr>
  </table>
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=bharqav&theme=tokyo-night&hide_border=true&bg_color=0d1117&color=38bdf8&line=0284c7&point=38bdf8" width="95%" alt="Activity Graph" />
</div>

<br/>

<!-- ================================================================= -->
<!-- 9. CURRENTLY DEEP-DIVING INTO                                     -->
<!-- ================================================================= -->

### 🔬 Currently Deep-Diving Into

1. **Speculative Decoding Acceptance Proofs**: Optimizing Leviathan rejection sampling across batched draft verification steps.
2. **Zero-Copy Memory-Mapped Weight Paging**: Eliminating page-fault penalties when executing sparse 30B MoE models on DRAM-constrained hardware.
3. **Lock-Free Ring Buffers & Actor Models**: Low-latency inter-process messaging over POSIX shared memory primitives.

<br/>

<!-- ================================================================= -->
<!-- 10. FOOTER & CONNECT                                              -->
<!-- ================================================================= -->

<div align="center">
  <a href="https://linkedin.com/in/bhargavpodapati">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  &nbsp;
  <a href="mailto:bhargavpodapati28@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  &nbsp;
  <a href="https://github.com/bharqav">
    <img src="https://img.shields.io/badge/GitHub-0d1117?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0d1117&height=70&section=footer" width="100%" alt="Footer Banner" />
</div>
