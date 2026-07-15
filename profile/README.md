<div align="center">

# MVL — Maximum Verifiable Language

**If your AI writes code without hesitation and your compiler guards the gate — why prove anything less than everything?**

</div>

---

MVL is a programming language where the compiler verifies **11 properties at compile time**. No null pointers. No buffer overflows. No data races. No unhandled errors. No secret leaks. If it compiles, it's correct.

| | What the compiler proves | What it prevents |
|---|---|---|
| **1** | Type safety | Impossible states |
| **2** | Memory safety | Use-after-free, buffer overflow |
| **3** | Exhaustive matching | Unhandled cases |
| **4** | Null elimination | Null pointer dereference |
| **5** | Error visibility | Silent error swallowing |
| **6** | Ownership | Double-free, resource leaks |
| **7** | Effect tracking | Hidden side effects |
| **8** | Termination | Infinite loops |
| **9** | Data race freedom | Concurrent access bugs |
| **10** | Refinement types | Out-of-range values |
| **11** | Information flow | Secret/tainted data leaks |

### Designed for AI generation

LLMs generate code effortlessly — annotations that are too tedious for humans (effect declarations, refinement predicates, ownership markers, information flow labels) are trivial for an LLM. MVL is designed for that world: the LLM handles the syntax, the compiler handles the proof.

### Get started

**Homebrew (macOS Apple Silicon):**

```sh
brew tap mvl-lang/mvl
brew install mvl
```

**Universal install script (all platforms, builds from source):**

```sh
curl -fsSL https://mvl-lang.org/install.sh | sh
```

```rust
fn double(x: Int where x > 0) -> Int where self > 0 {
    x * 2
}

fn main() ! Console {
    println(double(5).to_string())
}
```

### Links

| | |
|---|---|
| 🌐 Website | [mvl-lang.org](https://mvl-lang.org) |
| 📖 Documentation | [mvl-lang.org/getting-started](https://mvl-lang.org/getting-started/) |
| 💻 Compiler/Code | [github.com/mvl-lang/mvl](https://github.com/mvl-lang/mvl) |
| 🎯 Examples | [github.com/mvl-lang/examples](https://github.com/mvl-lang/examples) |
| 📊 Benchmark (incl. Owasp/CVE) | [github.com/mvl-lang/benchmark](https://github.com/mvl-lang/benchmark) |
| 📦 Install | `curl -fsSL https://mvl-lang.org/install.sh \| sh` |
| 📜 License | Apache-2.0 |
| 🏗️ Built by | [LAB271](https://github.com/LAB271) |
