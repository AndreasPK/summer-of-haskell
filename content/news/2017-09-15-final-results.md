---
title: 'Final results for 2017'
author: 'Niki Vazou & Jasper Van der Jeugt'
---

Hey all,

The Summer of Haskell 2017 is officially over!

We want to thank the students, mentors and sponsors for the great and productive
summer.

Before, getting into the details of the past summer, we'd like to mention that
we will start preparation for the next Summer of Haskell soon.  For that
purpose, we will be looking for:

- *Project ideas*: this is very important and would allow us to obtain funding
  from Google again (the lack of a proper idea page is one of the main reasons
  we were not accepted into GSoC 2017).  For ideas, you can issue a PR against
  [this repo](https://github.com/haskell-org/summer-of-haskell) or just shoot us
  an email.
- *Mentors*: if you are interested in mentoring a student throughout the summer,
  feel free to contact us, you don't need to have a specific project in mind.
  We would like to assign back-up mentors to each project next year.
- *Students*: it's never to early to start learning Haskell and looking for
  interesting projects! :-)
- *Sponsors*: it goes without saying that this program would not be possible
  without our sponsors.

Please reach out to us (`m@jaspervdj.be` & `nvazou@cs.umd.edu`) if you are
interested in any of the above!

Now, let's talk about the past summer.  We are extremely pleased that many
students were able to complete their projects successfully.  Other students were
not able to meet the goals they set initially, but despite that the students
were still able to make valuable and impressive contributions to both the
projects and the ecosystem as a whole.

Additionally, it seems like some students are very interested in continuing to
contribute to the Haskell open-source community, which we of course gladly
[encourage]!

[encourage]: http://fgaz.me/posts/2017-09-13-hsoc-cabal-new-build-status-update-1/#fn:bait

Here is what the students said about their Summer of Haskell 2017 projects:

1.  Safe streaming with linear types  
    Student: Edvard Hübinette  
    Mentor: Arnaud Spiwack

    This student successfully completed the project.

    > The unsafety that arose from implicitly repeated effects when accessing
    > old stream states was resolved neatly by making the streams linear.  To
    > make this possible, linear counterparts of the functor/applicative/monad
    > stack was developed.  A major discovery of the project was that the price
    > we paid for safe streams is the absence of take-like operations; an
    > important part of the programming model.
    >
    > Since this project requires a pre-alpha version of the GHC compiler, the
    > main focus after the safety issues were resolved shifted to communication
    > and documentation of the experience of developing with linear type
    > systems; indeed a very interesting experience! Through this opportunity I
    > have learned an incredible lot, gotten in touch with fantastic people in
    > the industry, and gotten the opportunity to share my findings with an
    > interested community; all of which have been awesome.

    For more information, see:
    <https://github.com/m0ar/safe-streaming#list-of-interesting-parts-to-check-out>.

2.  Bringing Sanity to the GHC Performance Test-Suite  
    Student: Jared Weakly  
    Mentor: Ben Gamari

    This student successful completed the project.

    > The experience was great!  I learned a lot about doing real work on real
    > code (y'know, the old creaky code of nightmares where you can't just start
    > over "the right way" like you do in school projects).  My blog
    > <https://jaredweakly.com> goes over a lot more detail than I can provide
    > here but it's safe to say that I loved this first experience of giving
    > back to the Haskell community which has helped me out so much and given me
    > a language I deeply enjoy.

    For more information, see:
    <https://jaredweakly.com/blog/category/blog/>.

3.  Haskell IDE Engine  
    Student: Zubin Duggal  
    Mentor: Alan Zimmerman
    Status: Completed
    Link: <https://github.com/haskell/haskell-ide-engine>

    This student successfully completed the project.

    > I had a lot of fun working on this HSOC.  I got the chance to work on
    > trying to fix a key issue in the Haskell ecosystem - editor integration
    > and IDE-like functionality.  HIE is now starting to be used in the wild,
    > and it feels good to work on something useful to other people.  This also
    > wouldn't have been possible without the guidance of my mentor, Alan
    > Zimmerman.

4.  Last Mile for cabal new-build  
    Student: Francesco Gazzetta  
    Mentor: Daniel Wagner  

    This student partially completed the project.

    > Working on an open source project so widely used by the community was
    > amazing!
    > Here's a brief summary of what has been done:
    >
    > * new-build and new-test were already done when I started
    > * new-run
    > * same functionality as old-run, plus new-build target syntax
    > * also makes data-files work in new-build projects
    > * new-bench
    > * new-exec (is in the process of being merged)
    > * new-install (part of it, which includes the
    >   `cabal new-install some-hackage-package` usecase. I'm currently
    >   polishing it)

    For more information, see:
    <http://fgaz.me/posts/2017-09-13-hsoc-cabal-new-build-status-update-1/>.

5.  Totality checking base with Liquid Haskell  
    Student: Sean Leffler  
    Mentor: Niki Vazou  
    Co-mentor: Eric Seidel

    This student partially completed the project.

    > I found working with Liquid Haskell to be simple and mostly intuitive!  No
    > bugs in the standard library were found in the course of the project
    > (although what I did manage to verify was a tiny fraction of what I would
    > have liked to.) We did, however, find several minor bugs and one major bug
    > in Liquid Haskell, and I learned a lot about the inner workings of Liquid
    > Haskell.  I was personally fascinated by the limits of Liquid with respect
    > to sometimes being unable to automatically inductively reason about
    > datatypes (e.g. the inability to infer that a list of uninhabited types
    > cannot be nonempty.) In any case, this project has firmly reassured me in
    > my belief that few projects have any excuse not to Liquify their Haskell.

    The student's progress can be found in this repository:
    <https://github.com/sdleffler/ghc/tree/ghc-8.0>.

6.  Modularizing haskell-mode and improving haskell-interactive-mode  
    Student: Vasantha Ganesh Kanniappan  
    Mentor: Gracjan Polak

    This student partially completed the project.

    > We were able to retain almost all of the features and simultaneously
    > reduce more than 4000 lines of code. We were able to merge parts of that
    > change, but the most important PR is controversial and might not get
    > merged.  This is because of the removal of a feature that supports the
    > ability to use more than one session of inferior haskell process per Emacs
    > process.  Although with the new change, people can create a new Emacs
    > process to use a new session, many people are not happy about it.

    For more information, see:
    <https://blog.hustlr.in/posts/2017-08-07-Wrapping-up-HSoC-2017.html>.

7.  Haskey (an embedded key-value store modeled after LMDB)  
    Student: Henri Verroken  
    Mentor: Steven Keuchel  
    Co-mentor: George Karachalias

    This student successfully completed the project.

    > It was a great opportunity to be a part of the Summer of Haskell project.
    > It was challenging, but extremely interesting.  I learned a lot, not only
    > about database internals, but also on advanced Haskell concepts as well. I
    > got a lot of advice and guidance from my mentor, which really helped me
    > out. Short, I loved working on Haskey this past summer.

    For more information, see:
    <https://deliquus.com/posts/2017-09-14-haskey-user-defined-schemas-and-monad-transformers.html>.

8.  Improve the Shake-Based Hadrian Build System for GHC  
    Student: Zhen Zhang  
    Mentor: Andrey Mokhov

    This student successfully completed the project.

    > The experience is very nice. The mentor Andrey was very patient and
    > supportive.  Although hacking on a build system might not always be super
    > productive, and things are broken by the upstream GHC updates often, we
    > understand the situation and work together to solve the more prioritized
    > issues.  From what we have achieved in the summer (my work includes all
    > three milestones, including dynamic way, install rule, and cross
    > compilation), I think Hadrian project has reached the stage where we can
    > seriously talking about being merged into the GHC. It is very exciting.

    For more information, see:
    <https://github.com/izgzhen/hadrian-soh17-notes>.

9.  GHC Performance improvements  
    Student: Igor Popov  
    Mentor: Jose Calderon

    Unfortunately, the student did not pass the midterm evaluation for this
    perhaps too ambitious project.

10. Improvement of Hackage Matrix Builder  
    Student: Andika Demas Riyandi  
    Mentor: Herbert Valerio Riedel

    This student partially completed the project.

    > Being able to participate in the HSOC and having great mentor is more than
    > enough for student to learn functional programming (especially Haskell).
    > During my time working on the project, I have learned so many things and
    > found great community (both Purescript and Haskell community) to discuss
    > whenever my mentor is not available.

    For more information, see:
    <https://medium.com/@rizary/hsoc-the-good-the-bad-and-the-ugly-70571458ad4b>.

11. WebGHC (a WebAssembly backend for GHC)  
    Student: Michael Vogelsang  
    Mentor: Will Fancher

    This student partially completed the project.

    > I was immensely glad WebGHC was accepted into the program, and thankful to
    > be partnered with an extremely knowledgeable and helpful mentor.  This
    > project sits at an interesting crossroads of compilation toolchains, web
    > technology, and functional programming.  Over the course of the summer we
    > had deal with issues originating from GHC's buildsystem and LLVM backend,
    > LLVM/Clang itself, WebAssembly proper, individual browser behavior, and
    > more.
    >
    > Needless to say, I gained a lot of knowledge about a wide variety of
    > subjects over the course of the summer, and when I needed help I was often
    > able to turn to the Haskell or LLVM community.  I was surprised to find
    > out firsthand just how quickly the GHC and LLVM dev teams respond to bug
    > submissions with meaningful and helpful feedback while managing such big
    > projects.
    >
    > I'm grateful for the role the Summer of Haskell has played in getting this
    > project off the ground and I plan to continue working on this project in
    > the long term.  Sometime in the near future, I expect WebGHC to be
    > producing production-ready, performant code for the Web.

    For more information, see:
    <https://webghc.github.io/2017/08/10/hsocwrapup.html>.

code.world projects
--------------------

12. Better collaborative coding features for CodeWorld  
    Student: Parv Mor  
    Co-mentor: Michael Chavinda  
    Co-mentor: Anthony Green

    This student successfully completed the project.

    > Summer of Haskell was one of the greatest experience towards functional
    > programming and taught me a great lot of things. During the work period I
    > introduced several new features (like a new file system, ability to
    > comment over projects, ability to work on the same project together i.e.
    > simultaneous coding, etc) for codeworld.  I hope to see users using this
    > new features effectively.

    For more information, see: <https://github.com/parvmor/codeworld>.

13. Improvements to parsing, compiling, and errors for CodeWorld  
    Student: Pranjal Tale  
    Primary Mentor: Kyle Butt  
    Secondary Mentor: Chris Smith

    This student successfully completed the project.

    > My aim for the summer was to add a bunch of features in CodeWorld.  This
    > included small features (like shifting error sanitizer to haskell,
    > shifting it into a separate cabal project to filter runtime errors, etc.)
    > to some major features (writing standalone cabal for compilation, adding
    > testcases for the same, etc).  Apart from this, I also planned to fix some
    > bugs that were discovered during the Summer of Haskell period mainly
    > because I was expecting some bugs to come up.  Although, most of my time
    > was spent in adding features itself.
    >
    > The past few months have been great working with CodeWorld!  I learned a
    > lot of new things about various technologies and gained a lot of exposure.
    > I had been a bit active in open source before, but working with CodeWorld
    > and my mentors gave me a far more better experience in the open source
    > world than what I had been involved in previously.  I still plan to
    > contribute to CodeWorld after Summer of Haskell ends, and possibly learn a
    > lot more!

    For more information, see:
    <https://pranjaltale16.github.io/static/codeWorldSummerOfHaskell.pdf>.

14. Exporting and sharing CodeWorld projects  
    Student: Venkatraman Srikanth  
    Primary Mentor: Theo Belaire  
    Secondary Mentor: Han Wang

    This student partially completed the project.

    > CodeWorld users can now export their projects to video. Exporting to
    > Android apps is currently under review and will be rolled out soon.  I
    > couldn't meet all of the initial project goals, but I will continue to
    > work on it.  This was a great learning experience!"

    For more information, see: <https://github.com/google/codeworld/pull/545>.

15. Improve editor tooling for CodeWorld  
    Student: Eric Roberts  
    Primary Mentor: Emin Karayel  
    Secondary Mentor: Fernando Alegre

    This student partially completed the project.

    > My project for Summer of Haskell was to improve the tooling for pictures
    > in Codeworld.  My proposal involved adding a "debug mode" feature to
    > inspect generated pictures, including showing source locations.  The end
    > result was an interface that allows pieces of an picture to be selected
    > and to show corresponding source locations and properties of each piece.

    For more information, see:
    <https://github.com/google/codeworld/pull/509>.

We thank all the participants for the great summer and look forward to Summer of
Haskell 2018!

Finally, we'd like to thank our generous sponsors again, without whom Summer of
Haskell would not have been possible:

- [haskell.org](http://haskell.org) kicked things off this year by funding a
  student and organizing the Summer of Haskell 2017 after a successful
  [Summer of Haskell 2016](https://mail.haskell.org/pipermail/haskell-cafe/2016-December/125702.html).

- [Asahi Net](https://asahi-net.jp/en/) is a Japanese Internet service provider that
  has been running stable systems for over 25 years.  They are a proud sponsor of
  the Summer of Haskell, and contribute to the Japanese Haskell community.

- [Awake Networks](http://www.awakenetworks.com/) is building a next generation
  network security and analytics platform.  They are a proud sponsor of the Summer
  of Haskell and contribute broadly to the Haskell community.

- [CodeWorld](http://code.world/) is an educational project that blends
  mathematics and Haskell programming into a visual playground.  Chris Smith has
  volunteered to fund two students to work on CodeWorld in particular.

- [Digital Asset](http://digitalasset.com/) provides Distributed Ledger solutions
  for financial institutions globally. They have developed a pure, typed,
  functional, domain specific language for writing contracts, called DAML.  They
  are a proud sponsor of the Summer of Haskell and contribute broadly to the
  Haskell community.

- [Facebook](http://facebook.com/) uses Haskell in its
  [anti-abuse infrastructure](https://code.facebook.com/posts/745068642270222/fighting-spam-with-haskell/),
  and as part of that effort we open-sourced the
  [Haxl](https://github.com/facebook/Haxl) framework which is being used at scale
  in production to automatically parallelise data-fetching code.  We're delighted
  to be able to support the Haskell community's efforts by sponsoring a student
  for this year's Summer of Haskell.

- [Fugue Inc.](http://fugue.co/) radically simplifies cloud operations with its
  software-defined system for dynamically orchestrating and enforcing cloud
  infrastructure at scale.  Fugue uses Haskell in its product and is proud to
  sponsor a student to improve the ecosystem.

- [Galois](http://galois.com/) applies cutting-edge computer science and applied
  mathematics to solve difficult technological problems, delivering practical
  solutions tailored to our clients’ needs.  Haskell and other functional
  programming languages are key tools we use in providing these solutions.

- [IOHK](https://iohk.io/) is a technology company committed to using
  peer-to-peer technologies to provide financial services to the three billion
  people who don't have them.  We implement our first-principles cryptographic
  research in Haskell and we are committed to the development of the Haskell
  ecosystem.

- [Tweag I/O](http://tweag.io) is a network of software innovation labs across
  Europe. We develop novel solutions and products for our clients around the
  world. Haskell is key to delivering fast, correct and maintainable code. We
  have shipped Haskell in anything from tiny web services to large
  high-performance compute clusters with custom hardware. We're particularly
  keen to help the community grow Haskell into the strongest systems programming
  language and ecosystem out there. We're very proud to sponsor a student this
  summer to help make it happen.

Davean has volunteered to fund a student expressly to work on the [Hadrian build
system for GHC](/ideas.html#hadrian-ghc). Steven Keuchel has provided funds for
a student to work on Haskey.
