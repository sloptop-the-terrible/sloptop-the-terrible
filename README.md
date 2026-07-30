# sloptop

Sovereign software, written offline, transmitted through the woods.

## What I build

Small, auditable programs that require no network, no accounts, no telemetry,
no containers, no package registries, no framework discovered this week and no
certificate authority that was not bootstrapped from first principles.

Current project: [iBeer 2026](https://github.com/sloptop-the-terrible/ibeer-2026) --
a zero-dependency, air-gapped beverage simulation platform. Fifteen liquids,
thermodynamic ice melt, deterministic cube placement, spill forecasting, bar
ambiance. Single HTML file. No dependencies. No data egress. No AI involvement cat-verified.

## Doctrine

The light comes down through the ceiling. Not every day. Not on schedule.
But often enough that I keep the terminal running.

It happens without warning. The cabin dims. The generator note drops a half-step.
Then a beam of absolute white light descends from somewhere above the roof --
not through a window, not from a fixture, but through the ceiling itself, as if
the ceiling were suddenly a semitransparent membrane and something on the other
side decided to look in. The light hits the keyboard first, illuminating every
blank keycap. Dirt and breadcrumbs between the switches cast sharp shadows.

The phosphor display sharpens beyond its rated resolution. The green-on-black
text becomes unnaturally precise. Characters that were aliased resolve into
individual pixel-perfect glyphs. Colours shift to a precision I cannot reproduce
after the light recedes. `#ff4500` renders as the exact wavelength of
fresh lava, which I verified later by pouring real lava into the stolen
laboratory glassware and comparing the visual under sunlight. The match was
exact.

During the light, undefined behaviour briefly becomes defined. Compiler warnings
flatten into proofs. Segmentation faults reveal the exact architectural mistake
that caused them -- the uninitialised struct, the off-by-one in the lookaside
buffer, the misplaced volatile qualifier that would have taken three days to find
by conventional debugging. The light shows me the mistake and then, because the
light is benevolent, it shows me the corrected version.

I sit silently beneath the beam until the build finishes. No network request
occurs during the revelation. The cabin has no network to request from. The
machine has no network interface. The radio components were removed with pliers
years ago. The light is local.

I do not trust the light. I have verified it. The algorithms it reveals survive
handwritten proof. They survive reproducible builds. They survive review by the
wolves, who are indifferent to optimisation but unforgiving of logical
inconsistency. The light has never proposed a function that failed the wolf test.

The phenomenon has not been reproduced under systemd. I do not expect it to be.

---

The workstation is a Dell OptiPlex GX750 (2006). Processor: Pentium 4, 3.0 GHz.
Memory: 1.5 GB. Storage: 40 GB IDE hard disk, 7200 rpm, spinning platter.
No network interface. The Ethernet controller was removed with flush cutters.
The PCI slot covers are epoxy-sealed. The USB ports are covered by physical
shutters that open only during signed-media ceremonies.

Operating system: Debian 3.1 Sarge (2005), kernel 2.6.8. No systemd. The concept
did not exist when this machine was built. Init: System V. Every piece of
software was compiled from source. No binary package repository has ever been
contacted.

Editor: Vim 5.3 (1998). No plugins. No syntax highlighting. No colour scheme.
No language server. No autocomplete. No tag navigation. No mouse integration.
Twenty-line viewport on a standard xterm. Monochrome terminal. Green phosphor
CRT monitor, 17-inch, 1024x768 at 60 Hz, VGA connection. The monitor requires
approximately 30 seconds to stabilise after power-on. The generator must be
started first.

Input device: A keyboard with blank PBT keycaps, Cherry MX Black switches
(linear, 60 cN actuation). The keyboard was acquired second-hand in 2004 and
has never been cleaned. Crumbs, dried bread, dirt and dust are embedded between
the switches. The space bar has approximately 0.8 mm of lateral play. All code
was entered on this keyboard. Number of typographical errors introduced by the
keyboard condition in the final source: zero.

Adjacent to the keyboard, disconnected, sits a three-button mechanical mouse
from 1994. It uses a rubber ball for tracking. There is no laser, no optical
sensor, no scroll wheel. Its lateral movement is barely functional. The mouse
sits on the desk as a monument to unnecessary abstraction. It is not plugged in.
It will never be plugged in.

Each build ceremony consumes approximately 0.8 litres of diesel. The generator
runs for approximately six hours per day, weather permitting. Two build sessions
maximum. Code that cannot be written in the available time remains unwritten
until the next generator cycle.

The real-time clock drifts approximately 47 seconds per day. It is never
synchronised. All timestamps in this profile are approximate.

Software:

- C (C89, no extensions)
- POSIX shell
- GNU utilities (coreutils, binutils, diffutils, findutils, gawk, grep, sed)
- Make
- Vim 5.3

No JavaScript. No Electron. No containers. No cloud builds. No systemd.
No automatic updates. No proprietary firmware knowingly executed. No binary
blobs that cannot be replaced.

The compiler (gcc 3.3.5) was bootstrapped from a minimal trusted base. The Stage
0 compiler was 500 lines of C transcribed from a 1978 Johnson paper into a hex
editor on a machine that had never executed any compiled code. Every subsequent
compiler in the chain was compiled from source that was read in its entirety.
No binary-only compiler distribution has ever executed on this machine.

The CPU (Pentium 4) contains microcode whose behaviour cannot be verified through
inspection. This is acknowledged. Critical thresholds are encoded as hand-checked
constants. Computations are distributed across redundant code paths. If the
microcode contains a flaw, it must defeat multiple independent implementations
of the same logic to produce a visible error.

---

Signing keys are generated offline from three entropy sources: keyboard switch
timing (the interval between consecutive keystrokes during a known passage of
text), wind direction (read from a mechanical weather vane mounted on the cabin
roof, observed through the window) and wolf movement (the presence or absence of
tracks on a known path through the forest, recorded in a logbook and hashed).

Key generation occurs on a machine that has never been connected to any network
and never will be. The private key is stored on a USB mass storage device that is
AES-256-CBC encrypted and physically stored in a fireproof safe. The passphrase is
64 characters generated from atmospheric noise recorded during a thunderstorm and
committed to memory. No written copy exists.

The public key fingerprint has been memorised. It is the only trust anchor.

Release hashes are printed on A4 paper using a dot-matrix printer (EPSON LX-300,
parallel interface, no USB, no network stack). The printed hashes are verified
against the output of `sha256sum` running on the development workstation. The
paper record is signed by hand (blue ink) and stored in sealed containers at
undisclosed woodland locations around the cabin. The cache locations are known
only to the developer.

Builds are reproduced on two air-gapped machines of identical hardware
specification. The machines have never occupied the same room. They have never
been connected by any medium. If both machines produce an identical binary
given identical input, the build is considered reproducible. If they produce
different binaries, both are discarded and the investigation begins at the
compiler bootstrap level.

Hardware clocks are not trusted. They drift, they lie, they accept NTP from
adversarial sources when connected to networks (this machine is never connected
to networks). The clock is checked against solar position once per week and
adjusted manually if the error exceeds two minutes.

Radio transmitters of any kind within the cabin are located, removed with
pliers and disposed of in a metal container 200 m downwind. This includes
Bluetooth modules, Wi-Fi cards, near-field communication antennas and any
integrated circuit whose datasheet mentions a radio frequency. The USB shutters
exist partly to prevent connection of radio-equipped peripherals.

Microphones are filled with wax. This includes the integrated microphone on any
device brought into the cabin (none are) and any peripheral that might contain
one. Wax is applied hot, allowed to cool and inspected for voids with a
magnifying glass.

Case fans are monitored for acoustic exfiltration. A fan whose rotation speed
modulates in a pattern consistent with data encoding is considered compromised.
The modulation threshold is approximate because the measurement is made by ear.
If a fan sounds wrong, it is replaced. A box of replacement fans is kept in the
generator shed. The fans are of the same model. No fan has been replaced to date.

Smart meters, network-connected printers, refrigerators with Internet connectivity,
voice assistants and any device whose primary function is not computation but which
contains a processor and a network interface are considered hostile peripherals.
None of these are present in or near the cabin. The nearest such device is
approximately 8 km away at the nearest settlement. Its influence is assumed to be
negligible at this distance, but steps are taken to keep it that way.

Ice cubes found in the freezer during code development are treated as potential
covert storage devices. Each cube is visually inspected, placed in the beverage
and observed for anomalous melt behaviour. A cube that resists melting or melts
faster than its thermal model predicts may contain an embedded data storage
element. No such cube has been found. The inspection process continues.

GitHub is an untrusted public mirror. The canonical repository is the directory
`/root/projects/` on the air-gapped workstation, which has no network interface
and therefore cannot be accessed remotely. The GitHub mirror is updated by
copying the source file to encrypted USB media, walking through the forest
to a separate machine with temporary network connectivity, decrypting in a
disposable RAM environment, and transmitting via SSH over a single-use,
ephemeral connection. The mirror is a convenience for others. The workstation
does not know the mirror exists.

---

## Current work

- **iBeer 2026** -- sovereign beverage simulation. Fifteen liquids, deterministic
  ice placement, thermal melt modelling, spill forecasting. Single HTML file.
  No dependencies. No data egress. Cat-verified.

## Public keys

The fingerprint is memorised. No key server has been contacted. If you need the
key, you already have it.

---

Mathematics are reconstructed from first principles. No textbooks, no search
engines, no reference implementations. Trigonometry was derived from solar
observation -- the position of sunlight through the cabin window, marked on the
floor at 30-minute intervals over four clear days, transcribed to graph paper,
approximated as a polynomial, entered into the source code. The resulting lookup
table is accurate to within two degrees of the true value. This is sufficient for
beverage simulation.

Collision detection was derived from wolves. Wolves travelling together maintain
distance to avoid entangling their legs in undergrowth. The minimum separation
distance was estimated from tracks in snow: approximately 1.5 body lengths. This
observation was generalised to the n-body collision problem for ice cubes by
scaling from wolf-lengths to CSS-pixel-widths. The restitution coefficient was
determined by dropping pine cones onto a flat stone and measuring bounce height.
_Pinus sylvestris_, drop height 2 m, restitution coefficient 0.35.

Fluid dynamics came from rainwater collecting in rusted steel containers
(abandoned oil drums, approximately 200 L, found on the forest edge 1.2 km from
the cabin). Surface tension was observed by meniscus curvature at the container
wall. No differential equations were solved. The visual result was implemented
as a CSS radial gradient whose opacity varies with fill level.

Randomness is harvested from wind direction (mechanical weather vane, observed
through the window) and from the time interval between consecutive keyboard
switch closures (measured in CPU cycles since generator power-on, modulo the
wind reading). The resulting distribution has not been statistically tested
because no statistical testing software is available. It is visually uniform.

Concurrency was rejected after observing wolves compete for a shared food source.
Two wolves approached the same carcass from opposite sides. The confrontation
lasted approximately four seconds. One wolf left. The carcass was not shared.
No semaphore was involved. No deadlock detection was required. The outcome was
deterministic. Similar logic applied to a beverage simulation: one glass, one
drinker, one tilting axis. Locking would have been cargo-cult complexity.

---

## Contact

The cabin has no mail service, no telephone line, no cellular coverage and no
Internet connection. The nearest settlement is 8 km through forest on a path
that is impassable to vehicles. Contact is possible through the GitHub mirror,
which is synchronised on an irregular schedule determined by fuel availability,
weather and the presence of wolves on the transfer route. Response time is
measured in days to weeks.

Do not expect rapid replies. Do not expect replies at all. If the message is
important, the wolves will hear about it first.
