# nvscene-presentation
yoloswag

## Outline
 - Requirements for a demo
   - Needs to run on SNES
   - Has to have awesome music
   - Has to have awesome sync
   - Has to look great

 - Music
   - SNES audio hardware
     - TODO
   - Existing SNES music tools
     - Official tools
       - Extremely hard (if not impossible) to find
       - Not that they would run on anything modern anyways
     - XMSNES
       - Converter tool from old tracker format to SNES blob + driver
       - Can track in any tracker that supports .xm
       - Hard to find
       - Not exactly WYHIWYG
         - Doesn't cover hardware compression
       - Doesn't support additional SNES features
         - Missing filtered echo, noise
   - Make my own!
     - 

 - Typical oldschool demo development process
   - Massive amounts of assembler

 - Am I supposed to meet all of my requirements this way?
   - Seriously? One coder in a reasonable amount of my spare time? In 2014?

 - I started to become OBSESSED with process
 - To be more specific, I started to become obsessed with MINIMIZING process
   - Just getting things to work isn't good enough anymore
   - I want to look back at my work and say "yes, this is elegant, this is pure. I'm proud of this."
   - This just isn't a sensation I get with C++ and assembler blobs.
     - Now of course, some of this is necessary
     - Concretions for our abstractions, the things we depend on, don't just materialize out of thin air
     - But the balance just doesn't feel right.

 - Let's talk about video compression
   - What is video?
     - A regular sequence of images
       - And by "regular" I mean regular intervals
     - How might we represent a video?
       - Obvious answer: Sequence of raw images

 - Chronological order of events:
   - Tried SNES dev at 15, couldn't do it
   - Did some C64 stuff, that was better
   - Back to SNES, not much progress
   - Kickassembler
   - Tried Atari VCS, made a custom sound driver, a few FX, but music sucked
   - Laptop stolen, tried Gameboy dev
   - Kickassembler too slow, custom assembler
   - Demon Blood
   - Revamped assembler
   - Started hand-coding FX for a demo
     - Scrollers etc
     - Mode7 rotozoomer
     - Lots more ideas, but the workflow sucked
   - Started designing awesome super snes tool
     - Emulated video hardware
     - Auto resource- and VRAM-management
       - Try to find old sketch?
   - SNES tracker
   - Nu
     - Cramped for time
     - Video
     - Typical demo workflow (GL, rocket)
     - Elix was born
   - Got bit by the functional bug
   - Smash It

## Additional gif links

http://ogawa-special.tumblr.com/post/44389730778
http://beastialthirst.tumblr.com/post/31577977794
http://rekall.tumblr.com/post/53336716531
http://rhubarbes.com/post/110259762466/bsr-02-by-peng-zhang-more-robots-here
http://mirkokosmos.tumblr.com/post/109219246332/by-yongsub-noh
http://cosmicwolfstorm.tumblr.com/post/107915138469/sketch2015-1-12-by-minovo-wang
http://www.motionaddicts.com/post/40884766462/cubism
http://www.motionaddicts.com/post/40884766462/cubism
http://bubblegumcrash.tumblr.com/post/87678344788/patlabor-1
http://cosmicwolfstorm.tumblr.com/post/77517558988/cyber-city-oedo-808
http://jump-gate.tumblr.com/post/66510035351

## Notes

 - Recall Gavin Strange's presentation from fitc. Consider putting the presentation together in a very designer-ish way, with vibrant colors, videos (gifs), etc in the presentation.

 - Take Bent's advice: Yes, get into the tech details; no, that's not the main focus. The main focus is the problem-solving side of things - inspire people to look at things differently, try new things, and take new perspectives.

 - Remember that this is a good opportunity to show YOU and what YOU're all about, not just one thing you did. Brand yourself with being awesome rather than the project in the talk. RADNESS.

 - Use Reveal.js (http://slides.com/) for the actual slides, possibly through https://github.com/fsprojects/FsReveal

 - Take inspiration also from the following talks:
   - https://www.youtube.com/watch?v=ubaX1Smg6pY
   - https://www.youtube.com/watch?v=rJosPrqBqrA

 - Get gifs from:
   - http://bits-and-pixels.tumblr.com/
   - http://waneella.tumblr.com/

## Original talk description

Ever wanted to make something that looks and sounds awesome with a gaming console you've played on your entire life? Ever wanted to build a proper, modern toolset to do so and experiment with functional programming at the same time? Then this talk is for you!

We'll take a look at two recent Super Nintendo demos, and, in particular, the ideas and methodologies applied when making them. First, we'll go over some of the details of the SNES' quirky hardware and the usual methods of making it tick. Building from there, we'll look at how most of this can be reduced to "simple" data processing, and how modern development techniques can be applied to make this simpler and more interesting.

All in all, this talk aims to show how applicable modern programming practices can be to unexpected problem domains, and how inspiring it can be to work with creative, out-of-the-box solutions. After all, a little ancient console dev never hurt anyone, right?
