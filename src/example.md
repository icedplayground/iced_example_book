# EXAMPLE

iced_hello_app
<br/>
🐱 [https://github.com/icedplayground/iced_hello_app](https://github.com/icedplayground/iced_hello_app)

```rust,ignore,iced
// 🧊 iced_hello_app
// src/main.rs
// src/main.rs
use iced::application;
use iced::widget::{center, text};
use iced::{Element, Result, Task};

#[derive(Default)]
struct App;

#[derive(Debug, Clone, Copy)]
enum Message {}

fn main() -> Result {
    application(App::update, App::view)
        .run_with(|| (App::default(), Task::none()))
}

impl App {

    fn update(&mut self, _message: Message) -> Task<Message> {
        Task::none()
    }

    fn view(&self) -> Element<'_, Message> {
        center(text("Hello, world!")).into()
    }
}


// ==================================
// copyright 2025 by nonresistant.near
```



---

copyright 2025 by nonresistant.near