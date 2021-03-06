stb
===

single-file public domain libraries for C/C++

library    | lastest version | category | description
--------------------- | ---- | -------- | --------------------------------
**stb_dxt.h** | 1.04 | 3D&nbsp;graphics | Fabian "ryg" Giesen's real-time DXT compressor
**stb_image.h** | 1.46 | graphics | image loading/decoding from file/memory: JPG, PNG, TGA, BMP, PSD, GIF, HDR, PIC
**stb_image_resize.h** | 0.90 | graphics | resize images larger/smaller with good quality
**stb_image_write.h** | 0.95 | graphics | image writing to disk: PNG, TGA, BMP
**stb_textedit.h** | 1.5 | UI | guts of a text editor for games etc implementing them from scratch
**stb_truetype.h** | 0.99 | graphics | parse, decode, and rasterize characters from truetype fonts

FAQ
---

#### What's the license?

These libraries are in the public domain (or the equivalent where that is not
possible). You can do anything you want with them. You have no legal obligation
to do anything else, although I appreciate attribution.

#### If I wrap an stb library in a new library, does the new library have to be public domain?

No.

#### A lot of these libraries seem redundant to existing open source libraries. Are they better somehow?

Generally they're only better in that they're easier to integrate,
easier to use, and easier to release (single file; good API; no
attribution requirement). They may be less featureful, slower,
and/or use more memory. If you're already using an equivalent
library, there's probably no good reason to switch.

#### Why "stb"? Is this something to do with Set-Top Boxes?

No, they are just the initials for my name, Sean T. Barrett.
This was not chosen out of egomania, but as a semi-robust
way of namespacing the filenames and source function names.

#### Will you add more image types to stb_image.c?

If people submit them, I generally add them, but the goal of stb_image
is less for applications like image viewer apps (which need to support
every type of image under the sun) and more for things like games which
can choose what images to use, so I may decline to add them if they're
too rare or if the size of implementation vs. apparent benefit is too low.

#### Are there other single-file public-domain libraries out there?

Yes. I'll put a list here when people remind me what they are.

#### Do you have any advice on how to create my own single-file library?

Yes. https://github.com/nothings/stb/blob/master/docs/stb_howto.txt

#### Why public domain?

Because more people will use it. Because it's not viral, people
are not obligated to give back, so you could argue that it hurts
the *development* of it, and then because it doesn't develop as
well it's not as good, and then because it's not as good, in the
long run maybe fewer people will use it. I have total respect for
that opinion, but I just don't believe it myself for most software.

#### Why C?

Primarily, because I use C, not C++. But it does also make it easier
for other people to use them from other languages.

#### Why not C99? stdint.h, declare-anywhere, etc.

I still use MSVC 6 (1998) as my IDE because it has better human factors
for me than later versions of MSVC.



