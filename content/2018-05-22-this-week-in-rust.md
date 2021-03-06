Title: This Week in Rust 235
Number: 235
Date: 2018-05-22
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

* [The Rust compiler is getting faster](https://blog.mozilla.org/nnethercote/2018/05/17/the-rust-compiler-is-getting-faster/).
* [Rand 0.5.0 released with quite significant changes over 0.4](https://www.reddit.com/r/rust/comments/8l95zk/rand_050_released/).
* [Cannoli: A Python compiler written entirely in Rust](https://github.com/joncatanio/cannoli).
* [Auto reloading development web servers with systemfd/listenfd](https://www.reddit.com/r/rust/comments/8kpea2/ann_auto_reloading_development_web_servers_with/).
* [Migrating to Actix Web from Rocket for stability](https://nbsoftsolutions.com/blog/migrating-to-actix-web-from-rocket-for-stability).
* [Improving SmallVec's speed by 60% and why that shouldn't matter to you](http://troubles.md/posts/improving-smallvec/).
* [Swapping and dropping to accelerate Rust in a benchmark](https://barrielle.cedeela.fr/research_page/dropping-drops.html).
* [Building a Datalog engine in under 300 lines of Rust](https://github.com/frankmcsherry/blog/blob/master/posts/2018-05-19.md).
* [Porting Rust benchmarks to Criterion](https://llogiq.github.io/2018/05/18/criterion.html).
* [Compile time prevention of SQL-injections in Rust](https://polyfloyd.net/post/compile-time-prevention-of-sql-injections/).
* [This week in Rust docs 106](https://guillaumegomez.github.io/this-week-in-rust-docs/blog/this-week-in-rust-docs-106).
* [The Embedded Working Group newsletter 5](https://internals.rust-lang.org/t/the-embedded-working-group-newsletter-5/7536).
* [podcast] [CoRecursive w/ Adam Bell - 013](https://corecursive.com/013-rust-and-with-jim-blandy). Rust and bitter C++ developers with Jim Blandy, one of the authors of Programming Rust.
* [podcast] [Rusty Spike Podcast - episode 29](https://rusty-spike.blubrry.net/2018/05/17/episode-29-may-16-2018/). Square, Amazon, the 1.26 release, Cloudflare, Rust???s birthday, and three-fold improvements.

# Crate of the Week

This week's crate is [Thunder](https://crates.io/crates/thunder), a crate for creating simple command-line programs. Thanks to [Bujiraso](https://users.rust-lang.org/u/Bujiraso) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [rustc-guide](https://github.com/rust-lang-nursery/rustc-guide) is a project to write a short guide about how the rust compiler works, and it needs your help. There are some [easier issues](https://github.com/rust-lang-nursery/rustc-guide/issues?q=is%3Aissue+is%3Aopen+label%3AEasy), [issues which might require a bit of investigation/code reading](https://github.com/rust-lang-nursery/rustc-guide/issues?q=is%3Aissue+is%3Aopen+label%3AMedium), and [issues which probably require some advanced knowledge or a lot of time](https://github.com/rust-lang-nursery/rustc-guide/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+label%3AHard).
* [annotate-snippets](https://github.com/zbraniecki/annotate-snippets-rs) - a crate for code snippets visual annotations (think: rustc error display) released 0.1 and is looking for code review, testing, and feedback.
* [Get started with these beginner-friendly issues](https://www.rustaceans.org/findwork/starters).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

140 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2018-05-14..2018-05-21

* [implement label break value](https://github.com/rust-lang/rust/pull/50045) (RFC [#2046](https://github.com/rust-lang/rfcs/blob/master/text/2046-label-break-value.md))
* [lexer: fix span override for the first token in a string](https://github.com/rust-lang/rust/pull/50924)
* [rustc: disallow modules and macros in expansions](https://github.com/rust-lang/rust/pull/50820)
* [prevent main from having a where clause](https://github.com/rust-lang/rust/pull/50782)
* [fix `fn main() -> impl Trait` for non-`Termination` trait](https://github.com/rust-lang/rust/pull/50656)
* [resolve: don't add unnecessary import candidates for `prefix::{self}` imports](https://github.com/rust-lang/rust/pull/50908)
* [rustc: introduce {ast,hir}::AnonConst to consolidate so-called "embedded constants"](https://github.com/rust-lang/rust/pull/50851)
* [fix conversion from Miri Value to ConstValue](https://github.com/rust-lang/rust/pull/50710)
* [unused shorthand field pattern finally fixed(?)](https://github.com/rust-lang/rust/pull/50854)
* [NLL: stop considering location when computing outlives relationships](https://github.com/rust-lang/rust/pull/50593)
* [NLL: use `reset_unifications` instead of creating new unification table](https://github.com/rust-lang/rust/pull/50874)
* [cleanup uses of TypeIdHasher and replace them with StableHasher](https://github.com/rust-lang/rust/pull/50531)
* [ensure derive(PartialOrd) is no longer accidentally exponential](https://github.com/rust-lang/rust/pull/50011)
* [review proc macro API 1.2](https://github.com/rust-lang/rust/pull/50473)
* [speed up the macro parser](https://github.com/rust-lang/rust/pull/50855)
* [speed up `opt_normalize_projection_type`](https://github.com/rust-lang/rust/pull/50818)
* [streamline `StringReader::bump`](https://github.com/rust-lang/rust/pull/50566)
* [tweak `nearest_common_ancestor()`](https://github.com/rust-lang/rust/pull/50649)
* [`CheckLoopVisitor`: also visit break expressions](https://github.com/rust-lang/rust/pull/50829)
* [don't lint numeric overflows in promoteds in release mode](https://github.com/rust-lang/rust/pull/50841)
* [add lint checks for unused loop labels](https://github.com/rust-lang/rust/pull/50763)
* [turn deprecation lint `legacy_imports` into a hard error](https://github.com/rust-lang/rust/pull/50760)
* [make the `const_err` lint `deny`-by-default](https://github.com/rust-lang/rust/pull/50653)
* [remove vestigial diverging !-coercion](https://github.com/rust-lang/rust/pull/50351)
* [reduce span highlighted code in unused_variables lint](https://github.com/rust-lang/rust/pull/50675)
* [update LLVM to fix performance regression](https://github.com/rust-lang/rust/pull/50827)
* [emit noalias on &mut parameters by default](https://github.com/rust-lang/rust/pull/50744) (hooray!)
* [add auto-impl for primitive type](https://github.com/rust-lang/rust/pull/50533)
* [fix an ICE when attempting to transmute an uninhabited type](https://github.com/rust-lang/rust/pull/50803)
* [fix an ICE when casting a nonexistent const](https://github.com/rust-lang/rust/pull/50788)
* [switch Vec from doubling size on growth to using RawVec's reserve](https://github.com/rust-lang/rust/pull/50739)
* [ensure that statics are always ByRef](https://github.com/rust-lang/rust/pull/50690)
* [don't unconditionally set CLOEXEC twice on every fd we open on Linux](https://github.com/rust-lang/rust/pull/50638)
* [improve format string errors](https://github.com/rust-lang/rust/pull/50610)
* [rustc_mir: allow promotion of promotable temps indexed at runtime](https://github.com/rust-lang/rust/pull/50603)
* [add Option::xor method](https://github.com/rust-lang/rust/pull/50553)
* [implement `[T]::align_to`](https://github.com/rust-lang/rust/pull/50319)
* [implement edition hygiene for keywords](https://github.com/rust-lang/rust/pull/50307)
* [add implementation of Extend for ()](https://github.com/rust-lang/rust/pull/50234)
* [implement From for more types on Cow](https://github.com/rust-lang/rust/pull/50170)
* [stabilize `num::NonZeroU*`](https://github.com/rust-lang/rust/pull/50808)
* [stabilize `inclusive_range_methods`](https://github.com/rust-lang/rust/pull/50758)
* [stabilize opt-level={s,z}](https://github.com/rust-lang/rust/pull/50265)
* [rustdoc: Add minification process](https://github.com/rust-lang/rust/pull/50632)
* [rustdoc: replace most (e)println! statements with structured warnings/errors](https://github.com/rust-lang/rust/pull/50541)
* [fix rustdoc panic with `impl Trait` in type parameters](https://github.com/rust-lang/rust/pull/50728)
* [compiletest: run revisions as independent tests](https://github.com/rust-lang/rust/pull/50400)

## New Contributors

* bstrie
* Daniel Mueller
* George Burton
* Jane Lusby
* Kyle Stachowicz
* Mikela
* Robin Krahl
* SHA Miao

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

* [disposition: merge] [Keyword unreservations (pure, sizeof, alignof, offsetof)](https://github.com/rust-lang/rfcs/pull/2421).
* [disposition: merge] [Unstable features accidentally usable on the Stable release chanel are still unstable](https://github.com/rust-lang/rfcs/pull/2405).
* [disposition: merge] [`#[used]` static variables](https://github.com/rust-lang/rfcs/pull/2386).
* [disposition: merge] [Allow `if let` guards in `match` expressions](https://github.com/rust-lang/rfcs/pull/2294).

## New RFCs

* [Reserve `f(a = b)` in Rust 2018](https://github.com/rust-lang/rfcs/pull/2443).

# Upcoming Events

The community team is trying to improve outreach to meetup organisers. Please fill out their [call for contact info](https://docs.google.com/forms/d/e/1FAIpQLSf52YXGhqBaHtCXtVna4iHYMK7IQaTqUW6V-ztsZC8C2TBInQ/viewform) if you are running or used to run a meetup.

* [May 24. Madrid, ES - Cuarto meetup de MadRust](https://www.meetup.com/MadRust/events/gfrdspyxhbgc/).
* **[May 27. Paris, FR - RustFest Paris 2018](https://paris.rustfest.eu/)**.
* [May 27. Mountain View, US - Open Table / Icebreaker: what projects are you working on](https://www.meetup.com/Rust-Dev-in-Mountain-View/events/glnfcpyxhbkc/).
* [May 29. Dallas, US - Last Tuesday Meetup](https://www.meetup.com/Dallas-Rust/events/zfgwzmyxhbmc/).
* [May 30/31. Berlin, DE - Rust/WASM course around JSConf.EU](https://ti.to/asquera-event-ug/rust-wasm-wwwtf-2018/).
* [May 30. Berlin, DE - Berlin Mozilla Meetup - Rust Hack and Learn](https://www.meetup.com/Berlin-Mozilla-Meetup/events/tvmmslyxhbnc/).
* [May 30. Rust Community Team Meeting at #rust-community on irc.mozilla.org](irc://irc.mozilla.org/rust-community).
* [May 30. Vancouver, CA - Rust Study/Hack/Hang-out night](https://www.meetup.com/Vancouver-Rust/events/ckwdlpyxhbnc/).
* [May 30. Milano, IT - Rust Exercises](https://www.meetup.com/rust-language-milano/events/250868847/).
* [Jun  2. Florian??polis, BR - 1?? Encontro Rust Floripa](https://www.meetup.com/rustfloripa/events/xvglrpyxjbdb/).
* [Jun  3. Mountain View, US - Open Table / Icebreaker: what projects are you working on](https://www.meetup.com/Rust-Dev-in-Mountain-View/events/glnfcpyxhbbc/).
* [Jun  5. Rust Community Content Subteam Meeting at #rust-content on irc.mozilla.org](irc://irc.mozilla.org/rust-content).
* [Jun  5. Johannesburg, ZA - Monthly Meetup of the Johannesburg Rustaceans](https://www.meetup.com/Johannesburg-Rust-Meetup/events/cpblrnyxjbhb/).
* [Jun  6. Rust Events Team Meeting](https://t.me/joinchat/EkKINhHCgZ9llzvPidOssA).
* [Jun  6. Rust Community Team Meeting at #rust-community on irc.mozilla.org](irc://irc.mozilla.org/rust-community).
* [Jun  6. Indianapolis, US - Indy.rs](https://www.meetup.com/indyrs/events/cpvshpyxjbjb/).
* [Jun  6. Atlanta, US - Grab a beer with fellow Rustaceans](https://www.meetup.com/Rust-ATL/events/rhvgrmyxjbjb/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*No jobs listed for this week.*

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

*No quote was selected for QotW.*

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42) and [llogiq](https://github.com/llogiq).*
