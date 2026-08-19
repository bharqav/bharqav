<!-- ================================================================= -->
<!-- 1. SPACE THEMED ANIMATED PROFILE HEADER                           -->
<!-- ================================================================= -->

<div align="center">
  <img src="https://raw.githubusercontent.com/bharqav/bharqav/main/assets/header.svg" width="100%" alt="Space Profile Header" />
</div>

<div align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&duration=2800&pause=1000&color=38BDF8&center=true&vCenter=true&multiline=false&width=700&height=40&lines=Building+baremetal+quantized+LLM+runtimes+in+portable+C99;Patching+VirtIO+hypervisor+transports+on+Microsoft+OpenVMM;Engineering+Raft-consensus+distributed+state+machines;Executing+fused+integer+GEMV+with+zero+hot-path+allocations" alt="Mission Control Typing SVG" />
  </a>
</div>

<div align="center">
  <p>
    <code>⚡ [MISSION: DEEP SPACE INFRASTRUCTURE] // APOGEE: 30B MoE // PERIGEE: 180MB RSS // WARP: AVX-512</code>
  </p>
</div>

<br/>

<!-- ================================================================= -->
<!-- 2. FLIGHT COMPUTER TELEMETRY                                      -->
<!-- ================================================================= -->

```c
/**
 * @file flight_computer.c
 * @brief Autonomous Deep-Space Guidance Computer & Host Telemetry.
 */

#include <stdio.h>
#include <stdint.h>

typedef struct {
    const char *commander;
    const char *station_role;
    const char *orbital_missions[4];
    const char *propulsion_kernel;
    uint32_t   telemetry_flags;
} nav_computer_t;

int main(void) {
    const nav_computer_t flight_deck = {
        .commander          = "Bhargav",
        .station_role       = "Systems and AI Infrastructure Engineer",
        .orbital_missions   = {
            "Baremetal Quantized LLM Runtimes (C99)",
            "Hypervisor Virtualization (VirtIO / OpenVMM)",
            "Container Propulsion (OCI / Cgroups v2)",
            "Distributed Clustered Consensus (Raft / WAL)"
        },
        .propulsion_kernel  = "Fused Integer GEMV on AVX2 / AVX-512 VNNI",
        .telemetry_flags    = (1 << 3) /* -O3 -march=native -fopenmp -Wall -Wextra */
    };

    printf("[%s] Station Status: ONLINE // Propulsion: %s\n", 
           flight_deck.commander, flight_deck.propulsion_kernel);
    return 0;
}
```

<br/>

<!-- ================================================================= -->
<!-- 3. PLANETARY CELESTIAL FLEET (FEATURED SYSTEMS)                   -->
<!-- ================================================================= -->

### 🪐 Planetary Fleet & Orbital Systems

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">🌌 <a href="https://github.com/bharqav/quantr-in-c">quantr-in-c</a></h3>
      <p><b>Zero-gravity baremetal quantized LLM and MoE runtime in portable C99.</b></p>
      <ul>
        <li><b>Zero Hot-Path Allocations</b>: Fused integer SIMD matrix multiplication using <code>_mm256_maddubs_epi16</code> and <code>_mm512_dpbusd_epi32</code>.</li>
        <li><b>15 Mathematical Test Gates</b>: Bit-exact parity verification across scalar and vectorized SIMD kernels.</li>
        <li><b>180MB RAM Floor</b>: Zero-copy virtual memory mapping and paged Q8_0 KV cache for memory-constrained hardware.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Orbit-Inner%20Core-0ea5e9?style=flat-square" />
        <img src="https://img.shields.io/badge/Lang-C99-00599C?style=flat-square&logo=c&logoColor=white" />
        <img src="https://img.shields.io/badge/SIMD-AVX512%20VNNI-orange?style=flat-square" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">🛰️ <a href="https://github.com/bharqav/mysh">mysh</a></h3>
      <p><b>POSIX command-line orbital flight deck and process control shell in C++.</b></p>
      <ul>
        <li><b>Recursive AST Propulsion</b>: Multi-stage pipeline execution (<code>|</code>), subshell branching, and file descriptor redirections.</li>
        <li><b>Process Group Control</b>: Terminal foreground and background signal routing with robust job isolation.</li>
        <li><b>Builtins & Resolution</b>: Native directory stack, alias substitution, and wildcard expansion.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Orbit-Outer%20Probe-10b981?style=flat-square" />
        <img src="https://img.shields.io/badge/Lang-C%2B%2B20-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
        <img src="https://img.shields.io/badge/Subsystem-POSIX%20Unix-red?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3 align="left">🪐 <a href="https://github.com/bharqav/distributed-kv-store">distributed-kv-store</a></h3>
      <p><b>Fault-tolerant clustered persistence engine from first principles.</b></p>
      <ul>
        <li><b>Raft Consensus Protocol</b>: Leader election, log replication, snapshotting, and cluster reconfiguration.</li>
        <li><b>Virtual Token Ring</b>: Consistent hashing for balanced data distribution and minimal partition rebalancing.</li>
        <li><b>Causal Ordering</b>: Hybrid Logical Clocks (HLC) with append-only Write-Ahead Logging (WAL).</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Orbit-Gas%20Giant-a855f7?style=flat-square" />
        <img src="https://img.shields.io/badge/Consensus-Raft-blueviolet?style=flat-square" />
        <img src="https://img.shields.io/badge/Lang-Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3 align="left">🔭 <a href="https://github.com/bharqav/ultimate-hybrid-rag">ultimate-hybrid-rag</a></h3>
      <p><b>High-throughput neural vector and lexical deep-space retrieval engine.</b></p>
      <ul>
        <li><b>Reciprocal Rank Fusion</b>: Blends dense neural vector embeddings with BM25 sparse lexical inverted indexes.</li>
        <li><b>Neural Reranking Pipeline</b>: Two-stage cross-encoder scoring with dynamic score normalization.</li>
        <li><b>Sub-10ms Latency</b>: Concurrent semantic chunking and zero-copy vector scoring.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Orbit-Deep%20Radar-yellow?style=flat-square" />
        <img src="https://img.shields.io/badge/Lang-Python%203.11-3776AB?style=flat-square&logo=python&logoColor=white" />
        <img src="https://img.shields.io/badge/Retrieval-Vector%20%2B%20BM25-blue?style=flat-square" />
      </p>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- 4. DEEP-SPACE OPEN SOURCE MISSIONS                                -->
<!-- ================================================================= -->

### 🌌 Deep-Space Open Source Missions

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🛡️ <a href="https://github.com/crucible-security/crucible">Crucible Security</a>: Tool Injection Assessment Engine</h4>
      <p><code>PR #64</code> (Issue #49) | <b>AI Red-Teaming Defense</b></p>
      <ul>
        <li>Built an adversarial attack module covering <b>OWASP AGENT-004 (Tool Misuse)</b> vulnerabilities across MCP-enabled agent fleets.</li>
        <li>Engineered 4 attack classes and 20 adversarial vectors simulating privilege escalation and tool output poisoning across <b>286+ passing tests</b>.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Security-OWASP%20AGENT--004-red?style=flat-square" />
        <img src="https://img.shields.io/badge/Protocol-MCP%20Trust%20Boundary-blueviolet?style=flat-square" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h4>🚦 <a href="https://github.com/crucible-security/crucible">Crucible Security</a>: CI/CD Security Policy Gating</h4>
      <p><code>PR #64</code> (Issue #52) | <b>Pipeline Enforcement</b></p>
      <ul>
        <li>Engineered a <code>--fail-on</code> severity threshold CLI flag to block deployment pipelines when findings meet or exceed target severity (HIGH, CRITICAL).</li>
        <li>Authored reusable GitHub Actions workflow templates for automated agent vulnerability scanning and report generation.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/CI%2FCD-Security%20Gating-red?style=flat-square" />
        <img src="https://img.shields.io/badge/Automation-GitHub%20Actions-blue?style=flat-square" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>🖥️ <a href="https://github.com/microsoft/openvmm">Microsoft OpenVMM</a>: VirtIO Spurious Interrupt Patch</h4>
      <p><code>PR #4226</code> | <b>Hypervisor Transport Core</b></p>
      <ul>
        <li>Fixed a spurious configuration-change interrupt emitted during the <code>DRIVER_OK</code> state transition by proving driver activation does not alter device configuration.</li>
        <li>Audited <code>INTx/MSI-X</code> and MMIO interrupt signaling paths, ensuring <code>config_generation</code> strictly increments only during <code>FEATURES_OK</code> negotiation.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Virtualization-VirtIO%20Core-0078D4?style=flat-square" />
        <img src="https://img.shields.io/badge/Lang-Rust%20Kernel-DEA584?style=flat-square&logo=rust&logoColor=white" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h4>📦 <a href="https://github.com/youki-dev/youki">youki</a>: OCI Live Memory & Cgroups v2 Controller</h4>
      <p><code>PR #3688</code> | <b>Container Runtime Subsystem</b></p>
      <ul>
        <li>Piped <code>--memory</code>, <code>--memory-reservation</code>, and <code>--memory-swap</code> through <code>LinuxMemoryBuilder</code> into the kernel cgroup controller layer.</li>
        <li>Corrected CLI types to signed <code>Option&lt;i64&gt;</code> to safely represent <code>-1</code> unlimited allocations, adding regression integration coverage for <code>memory.max</code>.</li>
      </ul>
      <p>
        <img src="https://img.shields.io/badge/Containers-OCI%20Runtime-orange?style=flat-square" />
        <img src="https://img.shields.io/badge/Linux-Cgroups%20v2-333333?style=flat-square&logo=linux&logoColor=white" />
      </p>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- 5. COSMIC TECH PROPULSION MATRIX                                  -->
<!-- ================================================================= -->

### ⚙️ Cosmic Propulsion Matrix

<table width="100%">
  <tr>
    <td width="25%" valign="top">
      <b>Stellar Cores</b><br/>
      <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=c,cpp,rust,go,python,ts" alt="Languages" /></a>
    </td>
    <td width="25%" valign="top">
      <b>Vector Thrusters (SIMD)</b><br/>
      <img src="https://img.shields.io/badge/SIMD-AVX2%20%2F%20AVX512-0284c7?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/ARM-NEON%20Intrinsics-0284c7?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/Concurrency-OpenMP%20%2F%20pthreads-0284c7?style=flat-square" /><br/>
      <img src="https://img.shields.io/badge/Memory-mmap%20%2F%20Zero--Alloc-0284c7?style=flat-square" />
    </td>
    <td width="25%" valign="top">
      <b>Orbital Comm Arrays</b><br/>
      <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=docker,linux,postgres,redis,git" alt="Infrastructure" /></a>
    </td>
    <td width="25%" valign="top">
      <b>Flight Deck Toolchain</b><br/>
      <a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=cmake,githubactions,bash,vscode" alt="Toolchain" /></a>
    </td>
  </tr>
</table>

<br/>

<!-- ================================================================= -->
<!-- 6. MISSION CONTROL TELEMETRY HUD                                  -->
<!-- ================================================================= -->

### 📊 Mission Control Telemetry HUD

<div align="center">
  <table border="0">
    <tr>
      <td>
        <img src="https://github-readme-stats.vercel.app/api?username=bharqav&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true&bg_color=050811&title_color=38bdf8&icon_color=38bdf8&text_color=94a3b8" width="410" alt="Telemetry Stats" />
      </td>
      <td>
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=bharqav&theme=tokyonight&hide_border=true&background=050811&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8&sideLabels=94a3b8&dates=64748b" width="380" alt="Orbital Streak" />
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bharqav&layout=compact&theme=tokyonight&hide_border=true&bg_color=050811&title_color=38bdf8&text_color=94a3b8&langs_count=8" width="500" alt="Language Distribution" />
      </td>
    </tr>
  </table>
</div>

<br/>

<!-- ================================================================= -->
<!-- 7. SUB-SPACE COMMUNICATIONS (CONTACT)                             -->
<!-- ================================================================= -->

<div align="center">
  <a href="https://linkedin.com/in/bhargavpodapati">
    <img src="https://img.shields.io/badge/Sub--Space_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  &nbsp;
  <a href="mailto:bhargavpodapati28@gmail.com">
    <img src="https://img.shields.io/badge/Quantum_Relay_Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  &nbsp;
  <a href="https://github.com/bharqav">
    <img src="https://img.shields.io/badge/Terminal_GitHub-050811?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=050811&height=70&section=footer" width="100%" alt="Footer Banner" />
</div>
