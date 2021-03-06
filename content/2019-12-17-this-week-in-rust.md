Title: This Week in Rust 317
Number: 317
Date: 2019-12-17
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts

* [Bisecting Rust compiler regressions with cargo-bisect-rustc](https://blog.rust-lang.org/inside-rust/2019/12/18/bisecting-rust-compiler.html).
* [Stop worrying about blocking: the new async-std runtime, inspired by Go](https://async.rs/blog/stop-worrying-about-blocking-the-new-async-std-runtime/).
* [From zero to main(): Bare metal Rust](https://interrupt.memfault.com/blog/zero-to-main-rust-1).
* [WASM as a platform for abstraction](http://adventures.michaelfbryan.com/posts/wasm-as-a-platform-for-abstraction/).
* [New gtk-rs release: Simplification and more of everything](https://gtk-rs.org/blog/2019/12/15/new-release.html).
* [Announcing Mio 0.7-alpha.1](https://tokio.rs/blog/2019-12-mio-v0.7-alpha.1/).
* [Introduction to Rendology: A Glium-based rendering pipeline](https://leod.github.io/rust/gamedev/rendology/2019/12/13/introduction-to-rendology.html).
* [The common Rust traits](https://stevedonovan.github.io/rustifications/2018/09/08/common-rust-traits.html).
* [Solving the Burger problem with Rust](https://rust-malaysia.github.io/code/2019/12/15/the-burger-problem.html).
* [Porting druid Rust widgets to PineTime smart watch](https://medium.com/@ly.lee/porting-druid-rust-widgets-to-pinetime-smart-watch-7e1d5a5d977a).
* [Relm tutorial](https://relm.antoyo.xyz/documentation/tutorial/).
* [Why does rust seem to inspire people](https://www.reddit.com/r/rust/comments/eaay3c/why_does_rust_seem_to_inspire_people/)?

# Crate of the Week

This week's crate is [bstr](https://github.com/BurntSushi/bstr), a string type for Rust that is not required to be valid UTF-8.

Thanks to [Willi Kappler](https://users.rust-lang.org/t/crate-of-the-week/2704/603) for the suggestions!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

*No issues were proposed for CfP*.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

223 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2019-12-09..2019-12-16

* [revert stabilization of never type](https://github.com/rust-lang/rust/pull/67224) (sorry ??? llogiq)
* [enable `loop` and `while` in constants behind a feature flag](https://github.com/rust-lang/rust/pull/67216)
* [make transparent enums more ordinary](https://github.com/rust-lang/rust/pull/67323)
* [ensure a hard error on generic ZST constants whose body causes an eval error](https://github.com/rust-lang/rust/pull/67134)
* [improve diagnostics and code for exhaustiveness of empty matches](https://github.com/rust-lang/rust/pull/67026)
* [do not ICE on unnamed future](https://github.com/rust-lang/rust/pull/67289)
* [remove the `DelimSpan` from `NamedMatch::MatchedSeq`](https://github.com/rust-lang/rust/pull/67250)
* [optimize `shallow_resolve_changed`](https://github.com/rust-lang/rust/pull/67079)
* [add ExactSizeIterator bound to return types](https://github.com/rust-lang/rust/pull/67125)
* [fix `-Z print-type-sizes`'s handling of zero-sized fields](https://github.com/rust-lang/rust/pull/67215)
* [track polonius in `-Z self-profile`](https://github.com/rust-lang/rust/pull/67193)
* [fix constant propagation for scalar pairs](https://github.com/rust-lang/rust/pull/67015)
* [fix `unused_parens` triggers on macro by example code](https://github.com/rust-lang/rust/pull/66983)
* [rustc: allow non-empty ParamEnv's in global trait select/eval caches](https://github.com/rust-lang/rust/pull/66821)
* [remove uniform array move MIR passes](https://github.com/rust-lang/rust/pull/66650)
* [chalk: remove depth getting passed around](https://github.com/rust-lang/chalk/pull/308)
* [chalk: when truncating a goal, don't truncate the environment](https://github.com/rust-lang/chalk/pull/294)
* [use first nonempty buffer in vectored I/O](https://github.com/rust-lang/futures-rs/pull/1998)
* [use deref target in Pin trait implementations](https://github.com/rust-lang/rust/pull/67039)
* [improve code generated for `starts_with('<literal char>')`](https://github.com/rust-lang/rust/pull/67249)
* [optimize `Ord` trait implementation for bool](https://github.com/rust-lang/rust/pull/66881)
* [inline some common methods on `OsStr`](https://github.com/rust-lang/rust/pull/67169)
* [`LinkedList`: drop remaining items when drop panics](https://github.com/rust-lang/rust/pull/67243)
* [`VecDeque`: drop remaining items on destructor panic](https://github.com/rust-lang/rust/pull/67235)
* [stabilize `Result::map_or`](https://github.com/rust-lang/rust/pull/66570)
* [add a separate path for messages with no format arguments](https://github.com/rust-lang/log/pull/366)
* [remove `NodeState::{Waiting,Done}`](https://github.com/rust-lang/rust/pull/66405)
* [match `VecDeque::extend` to `Vec::extend_desugared`](https://github.com/rust-lang/rust/pull/66341)
* [stabilize the `core::panic` module](https://github.com/rust-lang/rust/pull/66771)
* [`From<NonZero*>` impls for wider `NonZero` types](https://github.com/rust-lang/rust/pull/66277)
* [add str::strip_prefix and str::strip_suffix](https://github.com/rust-lang/rust/pull/66735)
* [cargo: emit error on `[target.'cfg(debug_assertions)'.dependencies]` and similar](https://github.com/rust-lang/cargo/pull/7660)
* [rustup: improve preinstalled rust message](https://github.com/rust-lang/rustup/pull/2155)
* [docs.rs: fix panic viewing source if crate failed to build](https://github.com/rust-lang/docs.rs/pull/519)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [RFC 2797: Announcing the FFI-unwinding Project Group](https://github.com/rust-lang/rfcs/pull/2797).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

*No RFCs are currently in final comment period.*

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Add IntoFuture trait and support for await](https://github.com/rust-lang/rust/pull/65244).
* [disposition: merge] [Add PartialEq and Eq to Cursor](https://github.com/rust-lang/rust/pull/67233).
* [disposition: merge] [Tracking issue for the `matches!` macro](https://github.com/rust-lang/rust/issues/65721).

## New RFCs

*No new RFCs were proposed this week.*

# Upcoming Events

### Europe

* [Dec 20. Stuttgart, DE - Meetup Stuttgart - Rust Hack and Learn](https://www.meetup.com/Rust-Community-Stuttgart/events/267063341/).
* [Jan  8. Berlin, DE - OpenTechSchool Berlin - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/nxdpgrybccblb/).

### North America

* [Dec 23. Durham, NC, US - Triangle Rustaceans - Project Night & Lightning Talks](https://www.meetup.com/triangle-rustaceans/events/mfglwpyzqbfc/).
* [Dec 31. Dallas, TX, US - Dallas Rust - Last Tuesday](https://www.meetup.com/Dallas-Rust/events/zfgwzmyzqbpc/).
* [Jan  1. Indianapolis, IN, US - Indy.rs](https://www.meetup.com/indyrs/events/mffbtpybccbcb/).
* [Jan  8. Atlanta, GA, US - Grab a beer with fellow Rustaceans](https://www.meetup.com/Rust-ATL/events/qxqdgrybccblb/).
* [Jan  8. Vancouver, BC, CA - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/qgvxlrybccblb/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Rust Developer for open-source work at Sigma Prime, Sydney, AU (Remote available)](https://lighthouse.sigmaprime.io/hiring-dec-2019.html).
* [WebAssembly and Compiler Engineer at NEAR, multiple locations (Remote available)](https://boards.greenhouse.io/near/jobs/4563917002).
* [Rust Developer at WarnerMedia, US](https://www.reddit.com/r/rust/comments/ebkyzc/need_a_rust_developer_on_a_6_month_contract/).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Hey @rustlang folks, is there a comprehensive writeup/reference anywhere of how the formatting machinery (format!(), write!(), etc.) work? Specifically from an implementation perspective (wrt trait objects, recursion)?

??? [James Munns](https://jamesmunns.com/blog/fmt-unreasonably-expensive/)

> It???s dark and ancient magic. I don???t think anyone knows it very well, never mind documentation

??? [Nick R. Cameron](https://twitter.com/nick_r_cameron/status/1203753952329650176?ref_src=twsrc%5Etfw)

Thanks to [mmmmib](https://users.rust-lang.org/t/twir-quote-of-the-week/328/756) for the suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42) and [llogiq](https://github.com/llogiq).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/ecuj74/this_week_in_rust_317/).</small>
