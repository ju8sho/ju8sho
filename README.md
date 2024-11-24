## Hi there 👋

```rust
use std::collections::HashMap;

struct JuSho;

struct Attributes;

impl Attributes {

    fn contact(&self) -> (String, String, String) {
        let telegram = "t.me/username".to_string();
        let channel = "t.me/channelname".to_string();
        let email = "username@example.com".to_string();
        (telegram, channel, email)
    }

    fn life(&self) -> (Vec<String>, u16) {
        let langs = vec!["Russian".to_string(), "Uzbek".to_string()];
        let birth_year = 1997;
        (langs, birth_year)
    }

    fn interests(&self) -> Vec<String> {
        let interests = vec![
            "Rust programming".to_string(),
            "Python programming".to_string(),
            "AI models and automation".to_string(),
            "Blockchain technology".to_string(),
            "Telegram bots development".to_string(),
            "Microcontrollers programming".to_string(),
            "Linux operating systems".to_string(),
            "Arch, Debian, Manjaro, Kali, Fedora, Ubuntu, Pop!_OS".to_string(),
        ];
        interests
    }

    fn coding(
        &self,
    ) -> (
        HashMap<String, Vec<String>>,
        Vec<String>,
        Vec<String>,
        HashMap<String, HashMap<String, HashMap<String, String>>>,
    ) {
        let mut langs = HashMap::new();
        langs.insert(
            "expert".to_string(),
            vec!["Python".to_string(), "Rust".to_string()],
        );

        let specialities = vec![
            "system programming".to_string(),
            "backend development".to_string(),
        ];

        let ide = vec!["VSCode".to_string(), "JetBrains".to_string()];

        let mut pc = HashMap::new();
        pc.insert(
            "Linux".to_string(),
            HashMap::from([(
                "Pop!_OS".to_string(),
                HashMap::from([
                    ("distro".to_string(), "Pop!_OS 22.04 LTS".to_string()),
                    ("desktop".to_string(), "GNOME".to_string()),
                ]),
            )]),
        );

        (langs, specialities, ide, pc)
    }
}

fn main() {
    let attributes = Attributes;

    let contact_info = attributes.contact();
    let life_info = attributes.life();
    let coding_info = attributes.coding();
    let interests_info = attributes.interests();

}
```
[![Rust](https://img.shields.io/badge/Rust-%23000000?style=for-the-badge&logo=rust&logoColor=white)](https://doc.rust-lang.org/)
[![Python](https://img.shields.io/badge/Python-%233776AB?style=for-the-badge&logo=python&logoColor=white)](https://docs.python.org/3/)

![Tasvir tavsifi](.ju8sho/diagram.svg)





