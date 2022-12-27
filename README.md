# Mapmaker

## Mapmaker/EXP 3.0 and Mapmaker/QTL

See the READ.ME for the original information from Whitehead Institute. As code
is refactored and bugs cleaned up, this README will evolve into the
Single-Source of Truth.

## Usage

TBD

## Build

TBD

## Contributing

See CONTRIB.md to understand the rules and requirements for contributing code.

## License

TBD, but probably GPL v3.0.

### Rationale
The original license for Mapmaker by Whitehead Institute was very specific to
Mapmaker - however there is a problem with that. Mapmaker incorporated GNU
readline and Ghostscript, both of which are GNU/GPL licensed. Without legal
assistance, I can't confirm that the original license can be adhered to and the
original license may have been in violation of the GNU/GPL.

## About

This repository is intended to be a rework of MAPMAKER/EXP 3.0, which was last
updated in 1993. Eventually the goal of the project is to rewrite the code into
something more modularized - preferably as a library that can be reused - and
will be differentiated from EXP/QTL as NG so as to clear up any confusion
between versions.

## Differences

At each official release (which will be tagged) the "DELTA.md" file will be
updated to include clear changes between MAPMAKER/NG and MAPMAKER/EXP. The
purpsoe of this will be to help academics and researchers to be able to
understand what exactly has changed and how it may affect their research.

### Supported Architectures

The original supported a wide range of systems and architectures, this work
will only support x86\_64 architecture running on Fedora Linux and other
Red Hat derivatives. Support for MacOS may come, however this work will not be
targeting ARM 64-bit until initial porting efforts and validation are
completed.

## Validation

This project will need help creating comprehensive tests that can help confirm
the implementation is accurate for research and that it could be cited in
research.

## Funding

This is being done purely as a labor of love, however if you do appreciate
what is being done, you may always send Bitcoin to
:moneybag:**3572USSPBj1FLNdA6T6GBHftH4hYdL1JiW**. If for some reason there is
need for new features or bug fixes to be prioritized, you can reach out to me
at sparticvs@popebp.com and we can discuss further (in the meantime I will look
for a bounty program system that can work for funds to be dedicated to the
first developer to complete the task).

## History

In 2008, I worked for the Rosen Center of Advanced Computing at Purdue
University as a Student Developer. One of my tasks was to update MAPMAKER/EXP
so that it would function on Windows XP. It took a little less than a year to
port the application to XP, and later needed to be ported again to Windows
Vista. I stopped working on the project at some point in late 2009/early 2010.

As a CS student, I learned a lot about programming from working on the port,
and at some point I decided I wanted to instead not only port it to Windows,
but port it to C#. There was a lot of work spent on the project, especially
with little actual knowledge of how I could properly make this work with the
intermixing of console output. Another goal I had along side this was to
parallelize the computation, as testing certain code-paths could take 4+ hours,
with the hope to reduce the time requirement.

During that time, I found a number of memory bugs in Mapmaker and other things
that worked only the first time and each subsequent run in interactive mode
would result in strange behavior. There was a lot of interest in the previous
work, but alas it was all lost to time.

~ sparticvs

