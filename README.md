<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,25,35,49&height=220&section=header&text=Bhargav&fontSize=68&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Systems%20%E2%80%A2%20Baremetal%20AI%20%E2%80%A2%20Distributed%20Infra&descFontSize=20&descAlignY=62&descAlign=50" width="100%" alt="Header Banner" />
</div>

<div align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&duration=2800&pause=1000&color=38BDF8&center=true&vCenter=true&multiline=false&width=650&height=40&lines=Building+baremetal+LLM+inference+engines+in+C99;Contributing+to+Microsoft+OpenVMM+%26+OCI+Container+Runtimes;Designing+Raft-consensus+distributed+key-value+stores;Writing+POSIX-compliant+shells+%26+low-latency+systems" alt="Typing SVG" />
  </a>
</div>

<div align="center">
  <p>
    ⚡ <i>"Premature optimization is the root of all evil — but mechanical sympathy is where the magic happens."</i>
  </p>
</div>

<br/>

<!-- ================================================================= -->
<!-- WHAT I'M BUILDING HOOK                                            -->
<!-- ================================================================= -->

<div align="center">
  <table>
    <tr>
      <td align="center" width="850">
        <b>🚀 Current Focus:</b> Writing zero-dependency quantized LLM/MoE inference runtimes (<b><a href="https://github.com/bharqav/quantr-in-c">Quantr</a></b>) executing 30B models in portable C99 with fused SIMD integer GEMV (< 200 MB peak RSS floor).
      </td>
    </tr>
  </table>
</div>

<br/>

<!-- ================================================================= -->
<!-- TERMINAL PROFILE GIMMICK                                          -->
<!-- ================================================================= -->

```c
/* sysinfo.c — Host Developer Identity */
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
    dev_t me = {
        .name           = "Bhargav",
        .role           = "Systems & AI Infrastructure Engineer",
        .core_focus     = { "Quantized LLM Runtimes (C99)", "Virtualization (VirtIO/OpenVMM)", 
                            "Container Runtimes (OCI/cgroups)", "Distributed Consensus (Raft)" },
        .current_kernel = "Fused Integer GEMV on AVX2 / AVX-512 VNNI",
        .favorite_flags = (1 << 3) /* -O3 -march=native -fopenmp -Wall -Wextra */
    };
    printf("%s: %s\n", me.name, me.role);
    return 0;
}
```

<br/>

<!-- ================================================================= -->
<!-- OPEN SOURCE CONTRIBUTIONS                                         -->
<!-- ================================================================= -->

### 🌐 Open Source Contributions

<table>
  <tr>
    <td>
      <h4>🛡️ <a href="https://github.com/crucible-security/crucible">Crucible Security</a> — Tool Injection Security Assessment Module (PR #64, Issue #49)</h4>
      <ul>
        <li><b>Adversarial Attack Engine</b>: Designed and implemented a dedicated Tool Injection assessment module expanding coverage for <b>OWASP AGENT-004 (Tool Misuse)</b> vulnerabilities across MCP-enabled and tool-augmented agent architectures.</li>
        <li><b>Attack Classes & Vectors</b>: Engineered <b>4 specialized attack classes</b> (<i>Parameter Injection, Selection Manipulation, Chain Poisoning, Unauthorized Invocation</i>) with <b>20 adversarial attack vectors</b> simulating privilege escalation, prompt-to-tool manipulation, and system prompt override attacks.</li>
        <li><b>Test Infrastructure</b>: Maintained full backward compatibility across <b>286+ passing unit and integration tests</b> with dynamic attack registration and centralized orchestration.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Security-OWASP%20AGENT--004-critical?style=flat-square" />
        <img src="https://img.shields.io/badge/Agentic%20AI-MCP%20Red--Teaming-blueviolet?style=flat-square" />
        <img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white" />
      </p>
    </td>
  </tr>
  <tr>
    <td>
      <h4>🚦 <a href="https://github.com/crucible-security/crucible">Crucible Security</a> — CI/CD Security Gating & Enforcement (PR #64, Issue #52)</h4>
      <ul>
        <li><b>Automated Pipeline Enforcement</b>: Implemented severity-based CI/CD gating by engineering a <code>--fail-on</code> threshold flag for the Crucible CLI, halting automated build pipelines on findings meeting or exceeding target severity (e.g. <code>HIGH</code>, <code>CRITICAL</code>).</li>
        <li><b>Reusable CI Action</b>: Created production-ready GitHub Actions workflow templates demonstrating automated agent vulnerability scanning, artifact reporting, and policy-driven build blocking.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/CI%2FCD-Security%20Gating-red?style=flat-square" />
        <img src="https://img.shields.io/badge/GitHub%20Actions-Workflow%20Automation-blue?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td>
      <h4>🖥️ <a href="https://github.com/microsoft/openvmm">Microsoft OpenVMM</a> — VirtIO DRIVER_OK Spurious Interrupt Elimination (PR #4226)</h4>
      <ul>
        <li><b>Transport Core Fix</b>: Identified and corrected a spurious VirtIO configuration-change interrupt emitted during the <code>DRIVER_OK</code> state transition, establishing that driver activation does not alter device configuration layouts.</li>
        <li><b>Interrupt Path Audit</b>: Audited <code>INTx/MSI-X</code> and MMIO interrupt signaling paths across MMIO and PCI transports, correcting test expectations and ensuring <code>config_generation</code> strictly increments only during <code>FEATURES_OK</code> negotiation.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Virtualization-VirtIO%20Core-0078D4?style=flat-square" />
        <img src="https://img.shields.io/badge/Rust-Systems%20Kernel-DEA584?style=flat-square&logo=rust&logoColor=white" />
        <img src="https://img.shields.io/badge/Hypervisor-OpenVMM-blue?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td>
      <h4>📦 <a href="https://github.com/youki-dev/youki">youki-dev / youki</a> — OCI Container Live Memory & Cgroups v2 Controller (PR #3688)</h4>
      <ul>
        <li><b>Dynamic Resource Updates</b>: Fixed CLI argument propagation in <code>youki update</code>, piping <code>--memory</code>, <code>--memory-reservation</code>, and <code>--memory-swap</code> through <code>LinuxMemoryBuilder</code> directly into the kernel cgroup controller layer.</li>
        <li><b>Unlimited Limits & Cgroups v2</b>: Corrected CLI types to signed <code>Option&lt;i64&gt;</code> to safely represent <code>-1</code> unlimited allocations, adding regression integration coverage for <code>memory.max</code>, <code>memory.low</code>, and <code>memory.swap.max</code>.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Containers-OCI%20Runtime-orange?style=flat-square" />
        <img src="https://img.shields.io/badge/Linux%20Kernel-Cgroups%20v2-333333?style=flat-square&logo=linux&logoColor=white" />
        <img src="https://img.shields.io/badge/Rust-Low--Level-DEA584?style=flat-square&logo=rust&logoColor=white" />
      </p>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- FEATURED PROJECTS                                                 -->
<!-- ================================================================= -->

### 🛠️ Featured Systems & Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">⚡ <a href="https://github.com/bharqav/quantr-in-c">quantr-in-c</a></h3>
      <p><b>High-Performance Quantized LLM & MoE Inference in Portable C99.</b></p>
      <ul>
        <li><b>Zero Dependencies</b>: No Python, no PyTorch, no BLAS, no CUDA runtime required.</li>
        <li><b>Fused SIMD GEMV</b>: Direct <code>_mm256_maddubs_epi16</code> & <code>_mm512_dpbusd_epi32</code> integer dot-products.</li>
        <li><b>Deterministic Verification</b>: 15 bit-exact mathematical test gates & paged Q8_0 KV cache.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/C99-00599C?style=flat-square&logo=c&logoColor=white" />
        <img src="https://img.shields.io/badge/SIMD-AVX2%2FAVX512-orange?style=flat-square" />
        <img src="https://img.shields.io/badge/LLM-GGUF-green?style=flat-square" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">🐚 <a href="https://github.com/bharqav/mysh">mysh</a></h3>
      <p><b>Production-Grade POSIX Mini-Shell in C++.</b></p>
      <ul>
        <li><b>Recursive AST Parser</b>: Multi-stage pipelines (<code>|</code>), subshells, and I/O redirections.</li>
        <li><b>Robust Job Control</b>: Custom foreground/background process group signaling and terminal control.</li>
        <li><b>Builtins & Globbing</b>: Native directory stack, alias substitution, and path wildcard expansion.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/C%2B%2B20-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
        <img src="https://img.shields.io/badge/POSIX-Unix-red?style=flat-square" />
        <img src="https://img.shields.io/badge/Systems-Process%20Trees-blue?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">📦 <a href="https://github.com/bharqav/distributed-kv-store">distributed-kv-store</a></h3>
      <p><b>Distributed, Fault-Tolerant Key-Value Store from First Principles.</b></p>
      <ul>
        <li><b>Raft Consensus</b>: Leader election, log replication, snapshotting, and cluster reconfiguration.</li>
        <li><b>Consistent Hashing</b>: Dynamic node ring with virtual tokens for uniform data distribution.</li>
        <li><b>Hybrid Logical Clocks</b>: Causal consistency ordering with append-only Write-Ahead Logging (WAL).</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Distributed-Raft-blueviolet?style=flat-square" />
        <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
        <img src="https://img.shields.io/badge/Storage-WAL%20Engine-teal?style=flat-square" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">🔍 <a href="https://github.com/bharqav/ultimate-hybrid-rag">ultimate-hybrid-rag</a></h3>
      <p><b>High-Throughput Vector + Lexical Hybrid Retrieval Engine.</b></p>
      <ul>
        <li><b>Fused Search</b>: Reciprocal Rank Fusion (RRF) combining dense vector embeddings & BM25 sparse indexes.</li>
        <li><b>Sub-10ms Latency</b>: Concurrent semantic chunking and cross-encoder neural reranking pipeline.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white" />
        <img src="https://img.shields.io/badge/RAG-Vector%20Search-blue?style=flat-square" />
        <img src="https://img.shields.io/badge/Embeddings-HuggingFace-yellow?style=flat-square" />
      </p>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- TECH STACK & ARSENAL                                              -->
<!-- ================================================================= -->

### ⚙️ Core Technical Arsenal

<table width="100%">
  <tr>
    <td width="25%" valign="top">
      <b>Core Languages</b><br/>
      <img src="https://skillicons.dev/icons?i=c,cpp,go,rust,python,ts" alt="Languages" />
    </td>
    <td width="25%" valign="top">
      <b>Systems & Compute</b><br/>
      <img src="https://img.shields.io/badge/SIMD-AVX2%20%2F%20AVX512-4C1D95?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/ARM-NEON%20Intrinsics-065F46?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/Concurrency-OpenMP%20%2F%20pthreads-1E40AF?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/Memory-mmap%20%2F%20Zero--Alloc-991B1B?style=flat-square" />
    </td>
    <td width="25%" valign="top">
      <b>Infrastructure & DBs</b><br/>
      <img src="https://skillicons.dev/icons?i=docker,linux,git,postgres,redis" alt="Infrastructure" />
    </td>
    <td width="25%" valign="top">
      <b>Toolchain & Build</b><br/>
      <img src="https://skillicons.dev/icons?i=cmake,githubactions,bash,vscode" alt="Toolchain" />
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- GITHUB METRICS & LIVE STATS                                       -->
<!-- ================================================================= -->

### 📊 Engineering Metrics & Telemetry

<div align="center">
  <table border="0">
    <tr>
      <td>
        <img src="https://github-readme-stats.vercel.app/api?username=bharqav&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true&bg_color=0d1117&title_color=38bdf8&icon_color=818cf8&text_color=94a3b8" width="410" alt="GitHub Stats" />
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

<br/>

<!-- ================================================================= -->
<!-- CONTRIBUTION GRAPH / ACTIVITY                                     -->
<!-- ================================================================= -->

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=bharqav&theme=tokyo-night&hide_border=true&bg_color=0d1117&color=38bdf8&line=818cf8&point=38bdf8" width="95%" alt="Activity Graph" />
</div>

<br/>

<!-- ================================================================= -->
<!-- CURRENTLY EXPLORING                                               -->
<!-- ================================================================= -->

### 🔬 Currently Deep-Diving Into
* 🧪 **Speculative Decoding Acceptance Proofs**: Optimizing Leviathan rejection sampling across batched draft verification steps.
* ⚡ **Zero-Copy Memory-Mapped Weight Paging**: Eliminating page-fault penalties when executing sparse 30B MoE models on DRAM-constrained hardware.
* 🦀 **Lock-Free Ring Buffers & Actor Models**: Low-latency inter-process messaging over POSIX shared memory.

<br/>

<!-- ================================================================= -->
<!-- FOOTER & CONNECT                                                  -->
<!-- ================================================================= -->

<div align="center">
  <a href="https://linkedin.com/in/bhargavpodapati">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  &nbsp;
  <a href="mailto:bhargavpodapati28@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  &nbsp;
  <a href="https://github.com/bharqav">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,25,35,49&height=80&section=footer" width="100%" alt="Footer Banner" />
</div>
