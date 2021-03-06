Title: This Week in Rust 323
Number: 323
Date: 2020-01-28
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

* [cargo-audit v0.11: Introducing the `fix` feature, yanked crate detection, and more](https://blog.rust-lang.org/inside-rust/2020/01/23/Introducing-cargo-audit-fix-and-more.html).
* [Bitfields forever: Why we need a C-compatible Rust crate](https://immunant.com/blog/2020/01/bitfields/).
* [Units of measure in Rust with refinement types](https://yoric.github.io/post/uom.rs/).
* [std.rs: go directly to stable rust docs](https://std.rs/).
* [A stack-less Rust coroutine library under 100 LoC](https://blog.aloni.org/posts/a-stack-less-rust-coroutine-100-loc/).
* [How Zebra used Tower to replace Zcash's legacy Bitcoin C++ networking code with modern, async Rust](https://www.zfnd.org/blog/a-new-network-stack-for-zcash/).
* [Build your own `block_on()`](https://stjepang.github.io/2020/01/25/build-your-own-block-on.html).
* [Packaging a Rust project for Debian](https://blog.hackeriet.no/packaging-a-rust-project-for-debian/).
* [Byte ordered streams](https://yoshuawuyts-blog.netlify.com/byte-ordered-stream-parsing/).
* [Tide channels](https://blog.yoshuawuyts.com/tide-channels/).
* [Lessons learnt updating a library to std::future](https://cetra3.github.io/blog/mpart-async-0-3-0/).
* [Returning trait objects](https://bryce.fisher-fleig.org/blog/returning-trait-objects/).
* [Debug Rust+Mynewt firmware for PineTime on Raspberry Pi](https://medium.com/@ly.lee/debug-rust-mynewt-firmware-for-pinetime-on-raspberry-pi-4b9ac2d093a9).
* [rust-analyzer changelog 9](https://rust-analyzer.github.io/thisweek/2020/01/27/changelog-9.html).

# Crate of the Week

This week's crate is [test-case](https://crates.io/crates/test-case), a framework for parameterized testing.

Thanks to [Synek317](https://users.rust-lang.org/t/crate-of-the-week/2704/712) for the suggestions!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [rust: fs::remove_dir_all rarely succeeds for large directories on windows](https://github.com/rust-lang/rust/issues/29497#issuecomment-573353391).
* [arcs: Interactive tools for drawing geometric items](https://github.com/Michael-F-Bryan/arcs/issues/9). Arcs is a Rust CAD System.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

261 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-01-20..2020-01-27

* [implement `?const` opt-out for trait bounds](https://github.com/rust-lang/rust/pull/68140)
* [unbreak linking with lld 9 on FreeBSD 13.0-CURRENT i386](https://github.com/rust-lang/rust/pull/68361)
* [export weak symbols used by MemorySanitizer](https://github.com/rust-lang/rust/pull/68410)
* [stabilize `#[repr(transparent)]` on `enum`s](https://github.com/rust-lang/rust/pull/68122)
* [fix `#[track_caller]` and function pointers](https://github.com/rust-lang/rust/pull/68302)
* [micro-optimize OutputFilenames](https://github.com/rust-lang/rust/pull/68409)
* [perf: avoid creating a SmallVec if nothing changes during a fold](https://github.com/rust-lang/rust/pull/68031)
* [suggest borrowing `Vec<NonCopy>` in for loop](https://github.com/rust-lang/rust/pull/68424)
* [further improve `impl Trait`/`dyn Trait` suggestions](https://github.com/rust-lang/rust/pull/68522)
* [typeck: simplify the handling of `diverges`](https://github.com/rust-lang/rust/pull/68422)
* [don't discard marker trait impls when inference variables are present](https://github.com/rust-lang/rust/pull/68057)
* [account for non-types in substs for opaque type error messages](https://github.com/rust-lang/rust/pull/68438)
* [avoid declaring a fake dependency edge](https://github.com/rust-lang/rust/pull/68298)
* [render const pointers in MIR more compactly](https://github.com/rust-lang/rust/pull/68516)
* [filter and test predicates using `normalize_and_test_predicates` for const-prop](https://github.com/rust-lang/rust/pull/68297)
* [make pointers to statics internal](https://github.com/rust-lang/rust/pull/68494)
* [avoid overflow in `std::iter::Skip::count`](https://github.com/rust-lang/rust/pull/68469)
* [simplify NodeHeader by avoiding slices in BTreeMaps with shared roots](https://github.com/rust-lang/rust/pull/67686)
* [add leading_ones and trailing_ones methods to the primitive integer types](https://github.com/rust-lang/rust/pull/68165)
* [futures: avoid starvation from FuturesUnordered::poll_next](https://github.com/rust-lang/futures-rs/pull/2049)
* [futures: add StreamExt::scan](https://github.com/rust-lang/futures-rs/pull/2044)
* [stdarch: add Icelake avx512 features](https://github.com/rust-lang/stdarch/pull/838)
* [cargo: store maximum queue length](https://github.com/rust-lang/cargo/pull/7829)
* [cargo: search for root manifest with ephemeral workspaces](https://github.com/rust-lang/cargo/pull/7768)
* [rustdoc: fix handling of compile errors when running `rustdoc --test`](https://github.com/rust-lang/rust/pull/68357)
* [docs.rs: fix various bugs in match_version](https://github.com/rust-lang/docs.rs/pull/565)
* [compiletest: simplify multi-debugger support](https://github.com/rust-lang/rust/pull/68391)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: merge] [target_feature 1.1](https://github.com/rust-lang/rfcs/pull/2396).
* [disposition: close] [Crate changelogs](https://github.com/rust-lang/rfcs/pull/2129).

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Correct inference of primitive operand type behind binary operation](https://github.com/rust-lang/rust/pull/68129).
* [disposition: merge] [Mutex and RwLock are unsound in presence of discriminant elision](https://github.com/rust-lang/rust/issues/68206).

## New RFCs

* [Rust 2020 roadmap](https://github.com/rust-lang/rfcs/pull/2857).
* [Secret Types](https://github.com/rust-lang/rfcs/pull/2859).
* [Project Groups](https://github.com/rust-lang/rfcs/pull/2856).

# Upcoming Events

### Europe

* [Feb  2. Brussels, BE - Rust devroom @ FOSDEM](https://fosdem.org/2020/schedule/track/rust/).
* [Feb  5. Berlin, DE - OpenTechSchool Berlin - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/nxdpgrybcdbhb/).
* [Feb  7. Darmstadt, DE - Rust Rhein-Main - Rust Meetup ??? Show Your Project](https://www.meetup.com/Rust-Rhein-Main/events/268145620/).
* [Feb 11. Zurich, CH - Rust Zurich - From cargo to kubernetes and back-up - February Meetup](https://www.meetup.com/Rust-Zurich/events/267790109/).

### North America

* [Feb  5. Vancouver, BC, CA - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/qgvxlrybcdbhb/).
* [Feb  5. Atlanta, GA, US - Rust Atlanta - Static Assertions Internals](https://www.meetup.com/Rust-ATL/events/qxqdgrybcdbqb/).
* [Feb  5. Indianapolis, IN, US - Indy.rs](https://www.meetup.com/indyrs/events/mffbtpybcdbhb/).
* [Feb 12. Houston, TX, US - Houston Linux Users Group - Rust Study Group](https://www.facebook.com/events/469382520642102).
* [Feb 12. Portland, OR, US - PDXRust - WASM: Run Rust in the browser](https://www.meetup.com/PDXRust/events/267797263/).
* [Feb 13. Columbus, OH, US - Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/dpkhgrybcdbrb/).
* [Feb 13. San Diego, CA, US - San Diego Rust February 2020 Meetup](https://www.meetup.com/San-Diego-Rust/events/268129845/).
* [Feb 18. Redmond, WA, US - Seattle Rust Meetup - Monthly meetup in Redmond](https://www.meetup.com/Seattle-Rust-Meetup/events/prbtdrybcdbpb/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Windows App Developer at 1Password, Toronto, ON, CA](https://1password.com/jobs/windows-developer/).
* [Rust Developer for privacy software at Cosmian, Paris (EU Remote available)](https://cosmian.com/were-hiring-developer-rust-cryptography-m-w-x/)
* [Systems Engineer (Rust) at Consensys, Remote](https://consensys.net/open-roles/1792013/).
* [Software Engineer at Open Analytics, Antwerp, BE](https://openanalytics.eu/jobs/OpenAnalytics_SoftwareEngineer.pdf).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Rust is basically Haskell's athletic younger brother. Not as intellectual, but still smart and lifts weights.

??? [icefox, Jan 22 in community-Discord #games-and-graphics](https://discordapp.com/channels/273534239310479360/335502453371961344/669636317277192222)

Thanks to [Duane](https://users.rust-lang.org/t/twir-quote-of-the-week/328/801) for the suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42) and [llogiq](https://github.com/llogiq).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/ew3gri/this_week_in_rust_323/).</small>
