# Box pointer

- example code to show that deref can move

    ```
    fn main() {
        let v: String = String::from("foobar");
        let v2 = &v;
        let v3 = *v2;
    
        println!{"{}, {}, {}", v, v2, v3};
    }
    ```

- another example of dref can move but not always in [this](https://users.rust-lang.org/t/why-dereferencing-moves-but-not-always/40204) link
