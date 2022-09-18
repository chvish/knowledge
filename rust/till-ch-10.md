# Traits
- Practice idea: implement a tiny prometheus library interface. Metric family as a trait, define the function each type should export etc.
- Implement trait for trait. The discussion turns to train object but for understanding the syntax, [this](https://stackoverflow.com/questions/29256519/i-implemented-a-trait-for-another-trait-but-cannot-call-methods-from-both-traits?noredirect=1&lq=1) question

# Lifetimes
- Add lifetime annotations to [this](https://play.rust-lang.org/?version=stable&mode=debug&edition=2021&gist=043c3192a0f1c9d26e8ac08d940517e9) program.

- How to read the lifetime syntax [link](https://stackoverflow.com/questions/68205578/clarification-on-rust-lifetime-syntax)

```
pub fn longest<'a>(x: &'a str, y: &'a str) -> &'a str 

// This doesn't mean that the lifetime of x and y is tied.
// Only that the lifetime of the output is tied to the lifetime
// of both of the inputs
```
- Why does compiler ask for `'static'` lifetime parameter for [this](https://stackoverflow.com/questions/40053550/the-compiler-suggests-i-add-a-static-lifetime-because-the-parameter-type-may-no?rq=1) program