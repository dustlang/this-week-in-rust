Title: This Week in Rust 142
Number: 142
Date: 2016-08-09
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta:
safety, concurrency, and speed. This is a weekly summary of its progress and
community. Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us an
email](mailto:corey@octayn.net?subject=This%20Week%20in%20Rust%20Suggestion)!
Want to get involved? [We love
contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts

* [Announcing Tokio](https://medium.com/@carllerche/announcing-tokio-df6bb4ddb34). A Finagle inspired network application framework for Rust.
* [Helping with the Rust errors](http://www.jonathanturner.org/2016/08/helping-out-with-rust-errors.html). Step-by-step instructions on how to help with the new Rust error messages.
* [Introduction to nom](http://hermanradtke.com/2016/08/08/introduction-to-nom-rust-parsing-combinator-framework.html). A parsing framework written in Rust.
* [Convenient and idiomatic conversions in Rust](https://ricardomartins.cc/2016/08/03/convenient_and_idiomatic_conversions_in_rust).
* [Better Exception Messages](http://os.phil-opp.com/better-exception-messages.html). Part of the series [Writing an OS in Rust](http://os.phil-opp.com/).
* [Writing a JPEG decoder in Rust](https://mht.technology/post/jpeg-rust-1/). Part 1: Background.
* [Extent of Intent](https://llogiq.github.io/2016/08/05/intent.html). Llogiq considers no-ops for consistency's sake harmful.
* [Rust code in mozilla-central now builds via cargo](https://groups.google.com/forum/#!topic/mozilla.dev.platform/BVPBhexRN3s).
* [imag usecases](http://beyermatthias.de/blog/2016/08/07/imag-usecases/). imag usecases explained.
* [podcast] [New Rustacean podcast episode 17](http://www.newrustacean.com/show_notes/e017/). A deep dive on references and pointers in Rust.

## New Crates & Project Updates

* [graph] Six months of rustc [performance](https://www.reddit.com/r/rust/comments/4w7e83/six_months_of_rustc_performance_201601_201606/) and [memory usage](https://www.reddit.com/r/rust/comments/4wk4uu/rustc_memory_usage/).
* [Tokamak 0.2.8 released](https://vertexclique.com/new-features-in-tokamak/). Now with Rustup support.
* Cargo nightly builds now [support vendoring dependencies](https://users.rust-lang.org/t/cargo-vendoring-now-on-nightly/6776).
* [Exar DB](https://github.com/bfil/exar-db). An event store with streaming support.
* [DUX](https://github.com/meh/dux). An X11 backlight manager.
* [rst](https://github.com/vitiral/rst). A requirements tracking tool made for developers and stands for "Requirements, Specifications and Tests". There is also an [introductory blog post](https://vitiral.github.io/developer/2016/08/08/why-hackers-should-track-their-requirements.html).
* [fdpass-rs](https://github.com/stemjail/fdpass-rs). A high level library to send and receive file descriptors through UNIX socket in a safe way.
* [This week in Servo 73](https://blog.servo.org/2016/08/01/twis-73/).
* [This week in Rust docs 16](https://guillaumegomez.github.io/this-week-in-rust-docs/blog/this-week-in-rust-docs-16).
* [This week in TiKV 2016-08-05](http://www.pingcap.com/tikv/2016/08/05/tikv-weekly/).
* [This week in Ruma 2016-08-07](https://www.ruma.io/news/this-week-in-ruma-2016-08-07/).

# Crate of the Week

This week's Crate of the Week is Dylan Ede's [rusttype](https://crates.io/crates/rusttype), a pure Rust freetype replacement. Thanks [mindtree](https://users.rust-lang.org/users/mindtree) for the suggestion.

[Submit your suggestions for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [easy] [rust book: Script to lint for copypasta'd file paths that should be generic](https://github.com/rust-lang/book/issues/123). Create a little script that will help the next version of the book have fewer errors!
* [easy] [rust: Error code list which need to be updated to new format](https://github.com/rust-lang/rust/issues/35233).
* [easy] [rustup: Don't capture backtraces without RUST_BACKTRACE=1](https://github.com/rust-lang-nursery/rustup.rs/issues/591#issuecomment-236235677).
  An easy fix, done in two steps, first modifying error-chain, then upgrading it in rustup.
* [easy] [rustup: Add command to install shell
  completions](https://github.com/rust-lang-nursery/rustup.rs/issues/387#issuecomment-234675568).
* [moderate] [rust: improve error message when resolution via Deref
  actually required
  DerefMut](https://github.com/rust-lang/rust/issues/28419). Good
  first type system bug.
* [hard] [imag: implement bindings to lua/lisp (ketos)/rhai for the filter
  library](https://github.com/matthiasbeyer/imag/issues/245)

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

147 pull requests were [merged in the last two weeks][merged].

[merged]: https://github.com/issues?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2016-08-01..2016-08-08

* Too many error description updates to report here
* [MIR switched on by default](https://github.com/rust-lang/rust/pull/34096) (test it while it's hot!)
* [MIR deaggregates struct access](https://github.com/rust-lang/rust/pull/35168)
* [The LLVM Upgrade from Hell](https://github.com/rust-lang/rust/pull/34743) (A most epic MIR blocker)
* [fix out-of-sync LLVM interface](https://github.com/rust-lang/rust/pull/35174)
* [Auto-Upgrade outmoded LLVM intrinsics](https://github.com/rust-lang/rust/pull/35261)
* [MinGW linking problems dodged](https://github.com/rust-lang/rust/pull/34830)
* [Fix `panic=abort` vs. plugins](https://github.com/rust-lang/cargo/pull/2954)
* [`TokenStream`s are now ropes](https://github.com/rust-lang/rust/pull/35018)
* [`TypeId`s are now unique cross-crate](https://github.com/rust-lang/rust/pull/35267)
* [Cross-Crate DefIds](https://github.com/rust-lang/rust/pull/35197) needed for MIR
* [Break unsound code with unused type parameters](https://github.com/rust-lang/rust/pull/35143) (breaking change, if you didn't infer that already)
* [Better warnings against shadowing types/imports](https://github.com/rust-lang/rust/pull/35116)
* [Ignore deprecated items within deprecated items](https://github.com/rust-lang/rust/pull/35317)
* [Unify inlined code caching](https://github.com/rust-lang/rust/pull/35114) (should need less RAM)
* [Unmatched surrogates are now reported in lowercase](https://github.com/rust-lang/rust/pull/35084) (could break your code if you relied on uppercase ??? hopefully no one did)
* [`impl From<Vec<char>>` and `From<&[char]> for String`](https://github.com/rust-lang/rust/pull/35054)
* [Handle `RwLock` reader overflow](https://github.com/rust-lang/rust/pull/35378)
* [Cargo now supports local registry mirrors](https://github.com/rust-lang/cargo/pull/2857)
* [Cargo warns, not errs on duplicate targets](https://github.com/rust-lang/cargo/pull/2962)


## New Contributors

* Adam Medzi??ski
* Alexander Altman
* Chris Stankus
* Christian Poveda
* Dominik Boehi
* Federico Ravasio
* Fran Guijarro
* Jakub Hlusi??ka
* Jared Wyles
* Jonathan Giddy
* kc1212
* m4b
* Matthias Rabault
* Mikhail Modin
* mLuby
* Moritz Ulrich
* Nick Massey
* Oliver Forral
* Omer Sheikh
* Peter C. Norton
* Rahul Sharma
* Roy Brunton
* Ryan Scott
* Samuel Cormier-Iijima
* Shantanu Raj
* silenuss
* Terry Sun
* TheZoq2
* trixnz
* Vincent Prouillet
* William Lee
* Yojan Shrestha
* Yossi Konstantinovsky

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now. [This week's FCPs][fcp] are:

[fcp]: https://github.com/rust-lang/rfcs/labels/final-comment-period

* [Create a team responsible for documentation for the Rust project](https://github.com/rust-lang/rfcs/pull/1683).
* [Add extra access methods for atomic types](https://github.com/rust-lang/rfcs/pull/1649).
* [Dedicated strike team to resolve unsafe code guidelines](https://github.com/rust-lang/rfcs/pull/1643).
* [Add a compiler flag that emits crate dependencies on a best-effort basis](https://github.com/rust-lang/rfcs/pull/1622).
* [Specify Rust compatibility of nursery crates](https://github.com/rust-lang/rfcs/pull/1619).
* [RFC process for formatting style and Rustfmt defaults](https://github.com/rust-lang/rfcs/pull/1607).
* [Define a best practices procedure for making bug fixes in the compiler](https://github.com/rust-lang/rfcs/pull/1589).
* [`FusedIterator` marker trait and `iter::Fuse` specialization](https://github.com/rust-lang/rfcs/pull/1581).
* [Add a `literal` fragment specifier for `macro_rules!` patterns that matches literal constants](https://github.com/rust-lang/rfcs/pull/1576).
* [Clarify the relationships between various kinds of structs and variants](https://github.com/rust-lang/rfcs/pull/1506).

## New RFCs

* [Allow crates to specify the version of Rust in which they are written](https://github.com/rust-lang/rfcs/pull/1709).
* [Support versioned dependencies on build tools, such as cargo](https://github.com/rust-lang/rfcs/pull/1707).
* [Add a 'thread lifetime, which denotes a thread-bounded region](https://github.com/rust-lang/rfcs/pull/1705).
* [Allow uncallable method impls to be omitted](https://github.com/rust-lang/rfcs/pull/1699).
* [Target bundles](https://github.com/rust-lang/rfcs/pull/1711). Combine distribution of standard libraries and targets into bundles for targeting a particular platform.

# Upcoming Events

* 8/10. Rust Community Team Meeting at #rust-community on irc.mozilla.org.
* [8/10. Rust Boulder/Denver Monthly Meeting](http://www.meetup.com/Rust-Boulder-Denver/events/232581073/).
* [8/11. Columbus Rust Society](http://www.meetup.com/columbus-rs/events/232469955/).
* [8/12. Frankfurt/Germany Meetup](http://www.meetup.com/de-DE/Rust-Rhein-Main/events/232956511/).
* [8/15. Rust Paris](http://www.meetup.com/Rust-Paris/events/230111511/).
* 8/17. Rust Community Team Meeting at #rust-community on irc.mozilla.org.
* [8/17. Rust Los Angeles Meetup](https://www.meetup.com/Rust-Los-Angeles/events/232933613/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email [Erick Tryzelaar][erickt] or [Brian
Anderson][brson] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[erickt]: mailto:erick.tryzelaar@gmail.com
[brson]: mailto:banderson@mozilla.com

# fn work(on: RustProject) -> Money

*No jobs listed for this week.*

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> The `if let` construction is a neat thing Rust borrowed from Swift (perhaps "copied" would be more accurate, or "cloned" depending on your views on whether ideas have owners).

??? [Frank McSherry in a blog post](https://github.com/frankmcsherry/blog/blob/master/posts/2016-08-03.md#differential-dataflow-internals-a-work-in-progress).

Thanks to [/u/vks_](https://www.reddit.com/r/rust/comments/4w1xlx/differential_dataflow_internals_a_work_in_progress/d65jvlh) and [Brian Anderson](https://users.rust-lang.org/t/twir-quote-of-the-week/328/278) for the suggestion.

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [brson](https://github.com/brson).*
