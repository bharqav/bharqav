<div align="center">

<img src="https://raw.githubusercontent.com/bharqav/bharqav/main/assets/header.gif" width="100%" alt="Bhargav - Systems and AI Infrastructure Engineer" />

<img src="https://img.shields.io/badge/-C99-0A0E14?style=for-the-badge&logo=c&logoColor=00D9FF" />
<img src="https://img.shields.io/badge/-C++-0A0E14?style=for-the-badge&logo=cplusplus&logoColor=00D9FF" />
<img src="https://img.shields.io/badge/-Rust-0A0E14?style=for-the-badge&logo=rust&logoColor=00D9FF" />
<img src="https://img.shields.io/badge/-Python-0A0E14?style=for-the-badge&logo=python&logoColor=00D9FF" />
<img src="https://img.shields.io/badge/-Linux-0A0E14?style=for-the-badge&logo=linux&logoColor=00D9FF" />

</div>

<br/>

<!-- SYSINFO -->
```c
/* engine.c - baremetal compute & runtime descriptor */
#include <stdint.h>
#include <immintrin.h>
#include <sys/mman.h>

typedef struct __attribute__((aligned(64))) {
    const char *identity;           /* "bhargav // systems & infrastructure" */
    const char *target_arch;        /* "x86_64 [avx-512 vnni] + aarch64 [neon]" */
    
    struct {
        uint32_t zero_copy_hugepages : 1;  /* mmap(MAP_SHARED | MAP_HUGETLB) */
        uint32_t fused_int4_gemv     : 1;  /* _mm512_dpbusd_epi32 tensor compute */
        uint32_t lockfree_ring_buf   : 1;  /* single-producer multi-consumer IPC */
        uint32_t raft_wal_sync       : 1;  /* O_DIRECT zero-amplification append */
        uint32_t reserved            : 28;
    } hw_caps;

    const char *active_pipeline[3];
    uint64_t    cache_miss_budget;         /* 0x0ULL - non-negotiable */
} compute_engine_t;

static const compute_engine_t host = {
    .identity    = "Bhargav -> Systems & AI Infrastructure Engineer",
    .target_arch = "x86_64 (AVX-512 VNNI) / aarch64 (NEON)",
    .hw_caps = {
        .zero_copy_hugepages = 1,
        .fused_int4_gemv     = 1,
        .lockfree_ring_buf   = 1,
        .raft_wal_sync       = 1,
    },
    .active_pipeline = {
        "Sub-200MB 30B MoE inference via memory-mapped KV paging",
        "Lock-free ring buffers & actor IPC over POSIX shared memory",
        "VirtIO interrupt auditing & custom kernel dispatch routines"
    },
    .cache_miss_budget = 0ULL
};
```

<br/>

## Open Source Contributions

<table width="100%">
<tr>
<td width="50%" valign="top">

**Crucible Security** - Tool Injection Assessment Module<br/>
`PR #64` · `Issue #49`

Built an adversarial attack engine covering OWASP AGENT-004 across MCP and tool-augmented agents. Four attack classes, twenty adversarial vectors, 286+ passing tests with dynamic attack registration.

`Python` `Security` `MCP`

</td>
<td width="50%" valign="top">

**Crucible Security** - CI/CD Security Gating<br/>
`PR #64` · `Issue #52`

Built a `--fail-on` severity threshold flag that blocks CI pipelines on HIGH/CRITICAL findings. Shipped reusable GitHub Actions templates for automated agent vulnerability scanning.

`CLI` `CI/CD` `GitHub Actions`

</td>
</tr>
<tr>
<td width="50%" valign="top">

**Microsoft OpenVMM** - VirtIO Interrupt Fix<br/>
`PR #4226`

Found and fixed a spurious config-change interrupt during the DRIVER_OK transition. Audited INTx/MSI-X/MMIO interrupt paths across transports and corrected `config_generation` increment behavior.

`Rust` `VirtIO` `Virtualization`

</td>
<td width="50%" valign="top">

**youki (OCI Runtime)** - Live Memory & cgroups v2<br/>
`PR #3688`

Fixed CLI argument propagation for `--memory`, `--memory-reservation`, and `--memory-swap` into the kernel cgroup layer. Corrected types to signed `Option<i64>` for unlimited allocations, added regression coverage.

`Rust` `cgroups` `OCI`

</td>
</tr>
</table>

<br/>

<div align="center">
  <img src="https://raw.githubusercontent.com/bharqav/bharqav/main/assets/pixel-art.gif" width="480" alt="Pixel Art" />
</div>

<br/>

## Featured Systems

<table width="100%">
<tr>
<td width="50%" valign="top">

### ⚡ quantr-in-c
Zero-dependency quantized LLM/MoE inference in portable C99.

- Fused SIMD GEMV using `_mm256_maddubs_epi16` and `_mm512_dpbusd_epi32`
- 15 bit-exact test gates, paged Q8_0 KV cache
- Sub-200MB peak RSS on 30B models

</td>
<td width="50%" valign="top">

### 🐚 mysh
Production-grade POSIX mini-shell in C++.

- Recursive AST parser for pipelines, subshells, redirection
- Real job control with foreground/background process groups
- Native directory stack, alias substitution, glob expansion

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📦 distributed-kv-store
Fault-tolerant distributed KV store from first principles.

- Raft consensus: leader election, log replication, snapshotting
- Consistent hashing with virtual tokens
- Hybrid logical clocks, append-only WAL

</td>
<td width="50%" valign="top">

### 🔍 ultimate-hybrid-rag
High-throughput hybrid vector and lexical retrieval engine.

- RRF fusion of dense embeddings and BM25 sparse indexes
- Cross-encoder neural reranking pipeline
- Sub-10ms latency on concurrent semantic chunking

</td>
</tr>
</table>

<br/>

## Technical Arsenal

<div align="center">

**Core Languages**
<br/>
<img src="https://skillicons.dev/icons?i=c,cpp,rust,python,go&theme=dark" />

**Systems & Compute**
<br/>
<img src="https://skillicons.dev/icons?i=linux,vim,bash&theme=dark" />

**Infrastructure & Data**
<br/>
<img src="https://skillicons.dev/icons?i=docker,kubernetes,redis,postgres,git&theme=dark" />

**Toolchain & Build**
<br/>
<img src="https://skillicons.dev/icons?i=cmake,gcc,github,githubactions&theme=dark" />

</div>

<br/>

## Currently Deep-Diving Into

- **Speculative decoding acceptance proofs** - optimizing rejection sampling across batched draft verification steps
- **Zero-copy memory-mapped weight paging** - eliminating page-fault penalties on sparse 30B MoE models under DRAM constraints
- **Lock-free ring buffers and actor models** - low-latency IPC over POSIX shared memory

<br/>

<div align="center">

<a href="https://linkedin.com/in/podapatibhargav"><img src="https://img.shields.io/badge/-LinkedIn-0A0E14?style=for-the-badge&logo=linkedin&logoColor=00D9FF" /></a>
<a href="mailto:bhargavpodapati28@gmail.com"><img src="https://img.shields.io/badge/-Email-0A0E14?style=for-the-badge&logo=gmail&logoColor=00D9FF" /></a>
<a href="https://github.com/bharqav"><img src="https://img.shields.io/badge/-GitHub-0A0E14?style=for-the-badge&logo=github&logoColor=00D9FF" /></a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0A0E14,100:1A2740&height=3&section=footer" width="100%"/>

</div>
