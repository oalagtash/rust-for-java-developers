# 🦀 Quick Dive into Rust — for Java Developers

**Learn Rust coming from Java**, through interactive lessons with side-by-side Java ↔ Rust code comparisons, Java→Rust mapping tables, and checkpoint quizzes — from `ArrayList` vs `Vec` to ownership, borrowing, and lifetimes.

**No build step, no dependencies, no signup.** One HTML file. Open it in a browser and start.

▶ **[Try it live](https://oalagtash.github.io/rust-for-java-developers/)** 

## Who this is for

You're an experienced **Java developer** (or Kotlin/JVM developer) who wants to **switch to Rust** or evaluate it — and you'd rather map new concepts onto what you already know than start from zero. Every lesson answers a concrete question you'll actually search for:

- What is the **Rust equivalent of `ArrayList`, `HashMap`, `Vector`, `StringBuffer`, or `Thread`**?
- How does **Rust ownership compare to Java garbage collection**?
- What replaces **`null` and `NullPointerException`** in Rust? (`Option<T>`)
- How do **Rust traits differ from Java interfaces**?
- What does Rust use instead of **exceptions and try/catch**? (`Result<T, E>` and `?`)
- How does **async/await compare to `CompletableFuture` and virtual threads**?
- Are **lifetimes** really that hard? (No — they're what the GC was doing for you, made visible)

## What's inside

**7 chapters · 19 lessons**, each with multiple annotated comparisons:

| Chapter | Topics |
|---|---|
| **Types & Data** | Primitives & integer overflow, `String` vs `&str` vs `StringBuilder`, collections (`ArrayList`→`Vec`, `HashMap` entry API vs `computeIfAbsent`), legacy synchronized types (`Vector`, `StringBuffer`, `Hashtable`), `Thread` / `AtomicInteger` / `ThreadLocal` |
| **Ownership** | Moves & `Drop` vs garbage collection, borrowing rules (goodbye `ConcurrentModificationException`), `Copy`/`Clone` & pass-by-value semantics |
| **Traits & Generics** | Traits vs interfaces (orphan rule, `#[derive]`), enums & pattern matching vs sealed interfaces + records, type erasure vs monomorphization, `dyn Trait` vs virtual dispatch |
| **Error Handling** | `Result<T, E>` & the `?` operator vs checked exceptions, `panic!` vs `RuntimeException` |
| **Concurrency** | Fearless concurrency with `Send`/`Sync`, `Arc<Mutex<T>>` vs `synchronized`, channels vs `BlockingQueue`, async/await vs `CompletableFuture` & Java 21 virtual threads |
| **Lifetimes** | Lifetime annotations explained as compile-time GC, elision rules, the `longest<'a>` pattern |
| **Ecosystem** | Cargo vs Maven/Gradle, crate equivalents (serde ≈ Jackson, tokio ≈ Netty, rayon ≈ parallel streams), built-in testing vs JUnit, doc tests |

Features: progress tracking, per-lesson quizzes, mapping tables, responsive layout, dark theme. Plain HTML/CSS/JS — no frameworks, works offline.

## Run it

```bash
# Option 1: just open the file
open index.html            # macOS
xdg-open index.html        # Linux

# Option 2: serve it
python3 -m http.server 8000
# → http://localhost:8000
```

## Host your own copy with GitHub Pages

1. Fork or push this repo to GitHub
2. **Settings → Pages → Source: Deploy from a branch → `main` / root**
3. Live at `https://<username>.github.io/<repo>/`

## FAQ

**Is Rust hard to learn for Java developers?**
The syntax is the easy part. The real shift is ownership and borrowing — which this course teaches by mapping them to things you already know: try-with-resources, `ConcurrentModificationException`, defensive copies, and what the GC silently does for you.

**Do I need to install Rust to use this?**
No. The lessons are self-contained comparisons. When you're ready to code, install via [rustup.rs](https://rustup.rs) and the Ecosystem chapter maps Cargo onto Maven/Gradle.

**Does this cover modern Java?**
Yes — comparisons use records, sealed interfaces, pattern-matching `switch`, `Optional`, Streams, `CompletableFuture`, and Java 21 virtual threads where relevant.

## License

[MIT](LICENSE) — use it, fork it, teach with it.

---

*Keywords: Rust tutorial for Java developers, learn Rust from Java, Java to Rust migration, Rust vs Java comparison, Rust equivalents of Java classes, interactive Rust course, Rust ownership explained, borrow checker, Rust for JVM developers.*
