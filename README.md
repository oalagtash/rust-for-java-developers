# 🦀 Rust for Java Experts

An interactive, single-file learning app that teaches Rust through the lens of Java — side-by-side code comparisons, Java→Rust mapping tables, and checkpoint quizzes.

## APP
https://oalagtash.github.io/rust-for-java-developers/ 

**No build step, no dependencies.** Just open `index.html` in a browser.

## What's inside

**7 chapters · 19 lessons**, each with multiple annotated comparisons:

| Chapter | Topics |
|---|---|
| **Types & Data** | Primitives & overflow, `String` vs `&str` vs `StringBuilder`, collections (`ArrayList`→`Vec`, `HashMap` entry API), legacy sync types (`Vector`, `StringBuffer`, `Hashtable`), `Thread` / `AtomicInteger` / `ThreadLocal` |
| **Ownership** | Moves & `Drop`, borrowing rules, `Copy`/`Clone` & function-call semantics |
| **Traits & Generics** | Traits vs interfaces (orphan rule, derives), enums & pattern matching vs sealed interfaces + records, type erasure vs monomorphization, `dyn Trait` |
| **Error Handling** | `Result<T, E>` & the `?` operator vs exceptions, `panic!` vs `RuntimeException` |
| **Concurrency** | `Send`/`Sync`, `Arc<Mutex<T>>`, channels vs `BlockingQueue`, async/await vs `CompletableFuture` & virtual threads |
| **Lifetimes** | Lifetimes as compile-time GC, elision, the `longest<'a>` pattern |
| **Ecosystem** | Cargo vs Maven/Gradle, crate equivalents (serde ≈ Jackson, tokio ≈ Netty, …), testing vs JUnit, doc tests |

Features: progress tracking, per-lesson quizzes, keyboard-free navigation, responsive layout, dark theme. Plain HTML/CSS/JS — no frameworks.

## Run it

```bash
# Option 1: just open the file
open index.html            # macOS
xdg-open index.html        # Linux

# Option 2: serve it
python3 -m http.server 8000
# → http://localhost:8000
```

## Host it with GitHub Pages

1. Push this repo to GitHub
2. **Settings → Pages → Source: Deploy from a branch → `main` / root**
3. Your app is live at `https://<username>.github.io/<repo>/`

https://oalagtash.github.io/rust-for-java-developers/ 

## License

[MIT](LICENSE)
