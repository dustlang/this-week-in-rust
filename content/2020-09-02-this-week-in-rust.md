Title: This Week in Rust 354
Number: 354
Date: 2020-09-04
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/emberian/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/emberian/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/emberian/this-week-in-rust/pulls).

# Updates from Rust Community

### Official
* [Announcing Rust 1.46.0](https://blog.rust-lang.org/2020/08/27/Rust-1.46.0.html)

### Tooling
* [Rust Analyzer Changelog #40](https://rust-analyzer.github.io/thisweek/2020/08/31/changelog-40.html)
* [Contributing to the IntelliJ Rust plugin: Writing an intention](https://kobzol.github.io/rust/intellij/2020/08/25/contributing-2-subst-assoc-type-int.html)

### Newsletters
* [Rust in Blockchain Newsletter #15 - Turbofish in the Blocksea](https://rustinblockchain.org/newsletters/2020-09-02-turbofish-in-the-blocksea/)

### Observations/Thoughts
* [Should we trust Rust with the future of systems programming?](https://edfloreshz.blog/should-we-trust-rust-with-the-future-of-systems-programming)
* [Optionality in the type systems of Julia and Rust](https://andreaskroepelin.de/blog/sum_types/)
* [Migrating from quick-error to SNAFU: a story on revamped error handling in Rust](https://dev.to/e_net4/migrating-from-quick-error-to-snafu-a-story-on-revamped-error-handling-in-rust-58h9)
* [Go use those Traits](https://prateeknischal.github.io/go-use-those-traits/)
* [Starframe devlog: Architecture](https://moletrooper.github.io/blog/2020/08/starframe-1-architecture/)
* [Event Chaining as a Decoupling Method in Entity-Component-System](https://www.jojolepro.com/blog/2020-08-20_event_chaining/)
* [Rust serialization: What's ready for production today?](https://blog.logrocket.com/rust-serialization-whats-ready-for-production-today/)
* [rust vs scripted languages; a short case study](https://www.linkedin.com/pulse/rust-goodness-case-study-matthew-sherborne)
* [DE] [Entwicklung: Warum Rust die Antwort auf miese Software und Programmierfehler ist](https://www.heise.de/hintergrund/Entwicklung-Warum-Rust-die-Antwort-auf-miese-Software-und-Programmierfehler-ist-4879795.html)
* [video] [Is Rust Used Safely by Software Developers?](https://youtu.be/iOBXVOAbpdY)

### Learn Standard Rust
* [Ownership in Rust, Part 1](https://www.thomascountz.com/2018/07/09/ownership-in-rust-part-1)
* [Ownership in Rust, Part 2](https://www.thomascountz.com/2018/07/11/ownership-in-rust-part-2)
* [Learning Rust 1: Install things and read a file](https://dev.to/jbachhardie/learning-rust-1-install-things-and-read-a-file-5613)
* [Learning Rust 2: A Tiny Database is Born](https://dev.to/jbachhardie/learning-rust-2-a-tiny-database-is-born-eef)
* [That's so Rusty: Ownership](https://dev.to/imaculate3/that-s-so-rusty-ownership-493c)

### Learn More Rust
* [As above, so below: Bare metal Rust generics 2/2](https://www.ecorax.net/as-above-so-below-2/)
* [Halite III Bot Development Kit in Rust](https://sgolem.com/halite-iii-bot-development-kit-in-rust)
* [Zero To Production #3.5: HTML forms, Databases, Integration tests](https://www.lpalmieri.com/posts/2020-08-31-zero-to-production-3-5-html-forms-databases-integration-tests/)
* [Objective-Rust](https://belkadan.com/blog/2020/08/Objective-Rust/)
* [Building web apps with Rust using the Rocket framework](https://blog.logrocket.com/rust-web-apps-using-rocket-framework/)
* [Writing an asynchronous MQTT Broker in Rust - Part 3](https://hassamuddin.com/blog/rust-mqtt/channels/)
* [Multiple Thread Pools in Rust](https://pkolaczk.github.io/multiple-threadpools-rust/)
* [Type-directed metaprogramming in Rust](https://willcrichton.net/notes/type-directed-metaprogramming-in-rust/)
* [Generating static arrays during compile time in Rust](https://dev.to/rustyoctopus/generating-static-arrays-during-compile-time-in-rust-10d8)
* [Let's build a single binary gRPC server-client with Rust in 2020 - Part 2](https://dev.to/tjtelan/let-s-build-a-single-binary-grpc-server-client-with-rust-in-2020-part-2-1i2e)
* [How to use Rust + WebAssembly to Perform Serverless Machine Learning and Data Visualization in the Cloud](https://www.freecodecamp.org/news/rust-webassembly-serverless-tencent-cloud/)
* [Fireworks for your terminal](https://blog.darrien.dev/posts/fireworks-for-your-terminal/)
* [Serverless Data Ingestion with Rust and AWS SES](http://jamesmcm.github.io/blog/2020/08/29/rust-ses/#en)
* [Box Plots at the Olympics](https://datacrayon.com/posts/programming/rust-notebooks/box-plots-at-the-olympics/)
* [Fixing include_bytes!](https://jack.wrenn.fyi/blog/include-transmute/)
* [Generating static arrays during compile time in Rust](https://dev.to/rustyoctopus/generating-static-arrays-during-compile-time-in-rust-10d8)
* [PL] [CrabbyBird #1 O tym, jak animowa?? posta?? gracza](https://postacnormalna.pl/animacja-kraboptaka/)
* [video] [FLTK Rust: Creating a music player with customized widgets](https://youtu.be/okdFx6tv7ds)

### Project Updates
* [This August in my database project written in Rust](https://alex-dukhno.github.io/2020-08-29-This-August-in-my-Database-project-written-in-rust-copy/)
* [Using Rust for Kentik's New Synthetic Monitoring Agent](https://www.kentik.com/blog/using-rust-for-kentiks-new-synthetic-network-monitoring-agent/)
* [AWS introduces Bottlerocket: A Rust language-oriented Linux for containers](https://www.zdnet.com/article/aws-introduces-bottlerocket-a-rust-language-oriented-linux-for-containers/)
* [Using `cargo test` for embedded testing with `panic-probe`](https://ferrous-systems.com/blog/cargo-test-with-panic-probe/)
* [Headcrab: August 2020 progress report](https://headcrab.rs/2020/08/31/august-update.html)
* [Rust Analyzer 2020[..6] Financial Report](https://rust-analyzer.github.io/blog/2020/08/20/financial-report.html)

### Miscellaneous
* [Avoid Build Cache Bloat By Sweeping Away Artifacts](https://www.justanotherdot.com/posts/avoid-build-cache-bloat-by-sweeping-away-artifacts.html)
* [const_fn makes it too easy to do mandelbrots](https://www.reddit.com/r/rust/comments/ijpxz2/const_fn_makes_it_too_easy_to_do_mandelbrots/)
* [Linux Developers Continue Evaluating The Path To Adding Rust Code To The Kernel](https://www.phoronix.com/scan.php?page=news_item&px=Linux-Kernel-Rust-Path-LPC2020)
* [Supporting Linux kernel development in Rust](https://lwn.net/SubscriberLink/829858/281103f9c6fd0dc2/)
* [video] [LPC 2020 - LLVM MC](https://youtu.be/FFjV9f_Ub9o)

* [Serverless Data Ingestion with Rust and AWS SES](http://jamesmcm.github.io/blog/2020/08/29/rust-ses/#en)

* [Refactoring Rust Transpiled from C](https://immunant.com/blog/2020/09/transpiled_c_safety/)

# Crate of the Week

This week's crate is [GlueSQL](https://github.com/gluesql/gluesql), a SQL database engine written in Rust with WebAssembly support.

Thanks to [Taehoon Moon](https://users.rust-lang.org/t/crate-of-the-week/2704/807) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [Database in Rust is looking for contributors](https://github.com/alex-dukhno/database/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22)
* [Docs.rs is looking for help adding a changelog](https://github.com/rust-lang/docs.rs/issues/1013)
* [Gooseberry has several good first issues with mentoring available](https://github.com/out-of-cheese-error/gooseberry/labels/good%20first%20issue)
* [Diskonaut - Option to delete without confirmation?](https://github.com/imsnif/diskonaut/issues/68)
* [Diskonaut - Feature: only show "(x = Small files)" legend when there are small files on the screen](https://github.com/imsnif/diskonaut/issues/15)
* [Diskonaut - Feature: error reporting with clean stacktraces](https://github.com/imsnif/diskonaut/issues/18)


If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

326 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-08-24..2020-08-31

* [point to a move-related span when pointing to closure upvars](https://github.com/rust-lang/rust/pull/75933)
* [abort when foreign exceptions are caught by `catch_unwind`](https://github.com/rust-lang/rust/pull/70212)
* [new pass to optimize `if` conditions on integrals to switches on the integer](https://github.com/rust-lang/rust/pull/75370)
* [suggest `mem::forget` if `mem::ManuallyDrop::new` isn't used](https://github.com/rust-lang/rust/pull/75912)
* [improve error message when typo is made in `format!`](https://github.com/rust-lang/rust/pull/75779)
* [allow reallocation to different alignment in `AllocRef`](https://github.com/rust-lang/rust/pull/75687)
* [add some avx512f intrinsics for mask, rotation, shift](https://github.com/rust-lang/stdarch/pull/884)
* [make some `Ordering` methods const](https://github.com/rust-lang/rust/pull/75463)
* [stabilize {`Range`, `RangeInclusive`}`::is_empty`](https://github.com/rust-lang/rust/pull/75132)
* [get rid of bounds check in `slice::chunks_exact()` and related functions](https://github.com/rust-lang/rust/pull/75936)
* [stdarch: avx512](https://github.com/rust-lang/stdarch/pull/887)
* [hashbrown: make `with_hasher` functions const fn](https://github.com/rust-lang/hashbrown/pull/195)
* [hashbrown: implement `replace_entry_with`](https://github.com/rust-lang/hashbrown/pull/190)
* [clippy: add a lint for an async block/closure that yields a type that is itself awaitable](https://github.com/rust-lang/rust-clippy/pull/5909)
* [use `rustc_lexer` for rustdoc syntax highlighting](https://github.com/rust-lang/rust/pull/75775)
* [report an ambiguity if both modules and primitives are in scope for intra-doc links](https://github.com/rust-lang/rust/pull/75815)
* [rustdoc: improve rendering of crate features via `doc(cfg)`](https://github.com/rust-lang/rust/pull/75330)
* [docs.rs: separate metadata parsing into a library](https://github.com/rust-lang/docs.rs/pull/1000)

## Rust Compiler Performance Triage

* [2020-08-31](https://github.com/rust-lang/rustc-perf/blob/master/triage/2020-08-31.md):
  1 regression, 2 improvements.
  
## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [RFC: Named arguments](https://github.com/rust-lang/rfcs/pull/2964)
* [eRFC: Add JSON backend to Rustdoc](https://github.com/rust-lang/rfcs/pull/2963)
* [RFC: Reading into uninitialized buffers](https://github.com/rust-lang/rfcs/pull/2930)

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge][Add `#[cfg(panic = '...')]`](https://github.com/rust-lang/rust/pull/74754)
* [disposition: merge][Allow Weak::as_ptr and friends for unsized T](https://github.com/rust-lang/rust/pull/74160)
* [disposition: merge][Update stdarch](https://github.com/rust-lang/rust/pull/73166)
* [disposition: merge][Tracking issue for #[doc(alias = "...")]](https://github.com/rust-lang/rust/issues/50146)

## New RFCs

* [Safer Transmute](https://github.com/rust-lang/rfcs/pull/2981)
* [[RFC]: Libs Team Governance](https://github.com/rust-lang/rfcs/pull/2979)
* [[RFC]: Portable SIMD Libs Project Group](https://github.com/rust-lang/rfcs/pull/2977)

# Upcoming Events

### Online
* [September 8. Saarbr??cken, DE - Rust-Saar Meetup - `3u16.map_err(...)`](https://www.meetup.com/Rust-Saar/events/272522454/)
* [September 8. Seattle, WA, US - Seattle Rust Meetup - Monthly meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrybcmblb/)
* [September 9. East Coast, US - Rust East Coast Virtual Talks + Q&A](https://www.meetup.com/Rust-NYC/events/272982073/)
* [September 11. Russia - Russian Rust Online Meetup](https://www.meetup.com/Rust-%D0%B2-%D0%9C%D0%BE%D1%81%D0%BA%D0%B2%D0%B5/events/272798484/)

### North America
* [September 9. Atlanta, GA, US - Rust Atlanta - Grab a beer with fellow Rustaceans](https://www.meetup.com/Rust-ATL/events/qxqdgrybcmbmb/)
* [September 10. Lehi, UT, US - Utah Rust - The Blue Pill: Rust on Microcontrollers (Sept / Second Round)](https://www.meetup.com/utah-rust/events/268567961/)

### Asia Pacific
* [September 7. Auckland, NZ - Rust AKL - Finally, good Rust IDE support in VSCode: rust-analyzer](https://www.meetup.com/rust-akl/events/266876702/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Senior Backend Engineer - Rust at Kraken (Remote US, Remote EMEA)](https://payward.wd1.myworkdayjobs.com/en-US/Kraken_Careers/job/EMEA---Remote/Senior-Backend-Engineer---Rust--Remote-_R-17)
* [Backend Engineer, Data Processing ??? Rust at Kraken (Remote US, Remote EMEA)](https://payward.wd1.myworkdayjobs.com/en-US/Kraken_Careers/job/AMER---Remote/Backend-Engineer--Data-Processing---Rust_L-43)
* [Backend Engineer - Rust at Kraken (Remote US, Remote EMEA)](https://payward.wd1.myworkdayjobs.com/en-US/Kraken_Careers/job/EMEA---Remote/Backend-Engineer---Rust_L-42)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> When the answer to your question contains the word "variance" you're probably going to have a bad time.

- [trentj on rust-users](https://users.rust-lang.org/t/in-this-mesh-class-whats-wrong-with-my-use-of-lifetimes/47946/4)

Thanks to [Michael Bryan](https://users.rust-lang.org/t/twir-quote-of-the-week/328/937) for the suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/imoogj/this_week_in_rust_354/)</small>
