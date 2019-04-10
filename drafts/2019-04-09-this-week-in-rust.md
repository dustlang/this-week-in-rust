Title: This Week in Rust 281
Number: 281
Date: 2019-04-09
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

The *This Week in Rust* privacy policy has changed due to our migration to GitHub pages for hosting. The current policy can be accessed [here](https://this-week-in-rust.org/pages/privacy-policy.html).

# Updates from Rust Community

## News & Blog Posts

[Array1 and function traits (Scientific computing: a Rust Adventure, Part 2)](https://www.lpalmieri.com/posts/2019-04-07-scientific-computing-a-rust-adventure-part-2-array1/).

# Crate of the Week

This week's crate is [interact](https://github.com/interact-rs/interact), a framework for online introspection of the running program state. Thanks to [Willi Kappler](https://users.rust-lang.org/t/crate-of-the-week/2704/513) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [rust: Add rustc-guide to toolstate](https://github.com/rust-lang/rust/issues/59597).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

198 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2019-04-01..2019-04-08

* [Show better errors for LLVM IR output](https://github.com/rust-lang/rust/pull/59744)
* [Use for_each to extend collections](https://github.com/rust-lang/rust/pull/59740)
* [wasi: Use shared API for preopened file descriptors](https://github.com/rust-lang/rust/pull/59727)
* [Never return uninhabited values at all](https://github.com/rust-lang/rust/pull/59639)
* [Shrink `mir::Statement`](https://github.com/rust-lang/rust/pull/59630)
* [Refactor async fn return type lowering](https://github.com/rust-lang/rust/pull/59286)
* [Unsized rvalues: implement boxed closure impls](https://github.com/rust-lang/rust/pull/59500)
* [Fixes for shallow borrows](https://github.com/rust-lang/rust/pull/59585)
* [Suggest using anonymous lifetime in `impl Trait` return](https://github.com/rust-lang/rust/pull/58919)
* [Fix invalid bounds string generation in rustdoc](https://github.com/rust-lang/rust/pull/58894)
* [More restrictive 2 phase borrows - take 2](https://github.com/rust-lang/rust/pull/58739)
* [Tweak `Span` encoding](https://github.com/rust-lang/rust/pull/58458)
* [Add 'partition_at_index/_by/_by_key' for slices](https://github.com/rust-lang/rust/pull/55448)
* [Support allocating iterators with arenas](https://github.com/rust-lang/rust/pull/59533)
* [Remove duplicated code from Iterator::{ne, lt, le, gt, ge}](https://github.com/rust-lang/rust/pull/59262)
* [Forward formatter settings to bounds of `Range<T>` in `fmt::Debug` impl](https://github.com/rust-lang/rust/pull/59596)
* [std: Avoid usage of `Once` in `Instant`](https://github.com/rust-lang/rust/pull/59676)
* [Improve worst-case performance of HashSet.is_subset](https://github.com/rust-lang/rust/pull/59665)
* [Improve worst-case performance of BTreeSet intersection](https://github.com/rust-lang/rust/pull/59186)
* [Implement useful steps_between for all integers](https://github.com/rust-lang/rust/pull/59444)
* [cargo: Add install-upgrade](https://github.com/rust-lang/cargo/pull/6798)
* [cargo: Improve error message to rerun a test in a workspace](https://github.com/rust-lang/cargo/pull/6824)
* [cargo Resolve: Be less strict while offline](https://github.com/rust-lang/cargo/pull/6814)
* [cargo: Add more suggestions on how to deal with excluding a package from a workspace](https://github.com/rust-lang/cargo/pull/6805)
* [Allow `cargo install --path P` to load config from P](https://github.com/rust-lang/cargo/pull/6804)
* [Allow `cargo doc --open` with multiple packages](https://github.com/rust-lang/cargo/pull/6803)
* [Speed up rustdoc run](https://github.com/rust-lang/rust/pull/59452)
* [crates.io: Add monitoring for common spam patterns](https://github.com/rust-lang/crates.io/pull/1678)


* [Add intial support for `wasm32-unknown-wasi`](https://github.com/rust-lang/libc/pull/1307)
* [Allow closure to unsafe fn coercion](https://github.com/rust-lang/rust/pull/59580)
* [Include bounds in generic re-ordering diagnostic](https://github.com/rust-lang/rust/pull/59572)
* [Optimize indentation in the pretty printer](https://github.com/rust-lang/rust/pull/59507)
* [Use `SmallVec` in `TokenStreamBuilder`](https://github.com/rust-lang/rust/pull/59476)
* [Make ASCII case conversions more than 4× faster](https://github.com/rust-lang/rust/pull/59283)
* [Adjust `MaybeUninit` API to discussions](https://github.com/rust-lang/rust/pull/59284)
* [Introduce `proc_macro::Span::source_text`](https://github.com/rust-lang/rust/pull/55780)
* [Add `Default` to `std::alloc::System`](https://github.com/rust-lang/rust/pull/59451)
* [Add `FromStr` impl for `NonZero` types](https://github.com/rust-lang/rust/pull/58717)
* [Implement `AsRawFd` for stdio locks](https://github.com/rust-lang/rust/pull/59512)
* [Simplify `checked_duration_since`](https://github.com/rust-lang/rust/pull/59374)
* [Stabilize `refcell_replace_swap`](https://github.com/rust-lang/rust/pull/59581)
* [stabilize `ptr::hash`](https://github.com/rust-lang/rust/pull/59603)
* [Stabilize {`f32`, `f64`}`::copysign()`](https://github.com/rust-lang/rust/pull/59503)
* [cargo metadata: Don't show `null` deps](https://github.com/rust-lang/cargo/pull/6534)
* [cargo install: Be more restrictive about cli flags](https://github.com/rust-lang/cargo/pull/6801)
* [rustdoc: Fix infinite recursion](https://github.com/rust-lang/rust/pull/59539)
* [rustdoc: collapse blanket impls in the same way as normal impls](https://github.com/rust-lang/rust/pull/59534)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [RFC 2657: Roadmap for 2019](https://github.com/rust-lang/rfcs/pull/2657).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: postpone] [Destructuring assignment](https://github.com/rust-lang/rfcs/pull/2649).

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [More restrictive 2 phase borrows - take 2](https://github.com/rust-lang/rust/pull/58739).
* [disposition: merge] [Tracking issue: const fn std::mem::needs_drop](https://github.com/rust-lang/rust/issues/51929).

## New RFCs

*No new RFCs were proposed this week.*

# Upcoming Events

### Asia Pacific

* [Apr 20. Beijing, CN - RustCon Asia](https://rustcon.asia/).

### Europe

* [Apr  4. Zagreb, HR - Rust Meetup 201904: Persistent data in Rust](https://www.meetup.com/Zagreb-Rust-Meetup/events/259597646/).
* [Apr  4. Wroclaw, PL - Rust Wroclaw Meetup](https://www.meetup.com/Rust-Wroclaw/events/259511136/).
* [Apr  4. Madrid, ES - Madrid Rust Meetup](https://www.meetup.com/MadRust/events/259988070/).
* [Apr 13. Kyiv, UA - PeerLab Kyiv #NativeDev: Rust 1.34 Release in Depth](https://www.meetup.com/PeerLab-Native-Developers/events/260050471/).
* [Apr 17. Berlin, DE - Berlin Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/gkkttqyzgbwb/).
* [Apr 18. Turin, IT - Mozilla Torino - Gruppo di studio Rust](https://www.meetup.com/Mozilla-Torino/events/ktqcpqyzgbhc/).

### North America

* [Apr  9. Seattle, US - Seattle Rust Meetup - Monthly meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/nzfspqyzgbmb/).
* [Apr  9. Irvine, US - Orange County Rust - C2Rust - Rewrite all the things](https://www.meetup.com/oc-rust/events/260233390/).
* [Apr 11. Arlington, US - Rust DC — Mid-month Rustful](https://www.meetup.com/RustDC/events/259782531).
* [Apr 11. Columbus, US - Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/dbcfrpyzgbpb/).
* [Apr 18. Denver, US - Rust Boulder/Denver - Rust Meetup for April](https://www.meetup.com/Rust-Boulder-Denver/events/259124388/).
* [Apr 17. Vancouver, CA - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/gqbksqyzgbwb/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Rust Developer at Smarkets, London, UK](https://smarkets.com/job/1617761/).
* [Database Engine Developer at Parity, Berlin, DE](https://www.parity.io/jobs/#berlin-database-engine-developer).
* [Lead Engineer (Cryptography) at Cosmian, Paris, FR](https://cosmian.com/wp-content/uploads/2019/03/Rust-CPP-lead-engineer.pdf).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

Sadly there was no suggestion this week.

[Please submit your quotes for next week](http://users.rust-lang.org/t/twir-quote-of-the-week/328)!

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [Flavsditz](https://github.com/Flavsditz).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/b93t3p/this_week_in_rust_280/).</small>