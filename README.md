# lloid
**L**au's Open-Source Voca**loid**/Utau**loid** Clone.

## Workspace
This project is organized into a workspace with multiple crates:

 - [lloid](lloid/) - Main lloid application
 - [lloid_twang](lloid_twang/) - Computer Voice Synthesizer
 - [lloid_voice](lloid_voice/) - Lloid Voice Format
 - [lloid_splice](lloid_splice/) - Voice Splicing
 - [lloidoid](lloidoid/) - Lloidoid Graphics

## Writing Songs
The synthesis engine will require you write lyrics phonetically.  Lloid uses a
custom simplified phonetic alphabet based on ascii.  There are 6 extra vowel
sounds, written with multiple letters - making 32 unique sounds.  The engine
will be able to create approximates and diphthongs from these 32 sounds (marked
with bullet points).

Lloid uses 4 different categories for sounds:

### Vowels
0. a - au (fault) `falt`
1. ah - a (large) `lahrdj`
2. e - ie (friend) `frend`
3. eh - ai (chair) `tcehr`
4. i - ea (sea) `si`
5. ih - i (sit) `siht`
6. o - o (rock) `rok`
7. oh - o (stone) `stohn`
8. u - oo (soon) `sun`
9. uh - oo (book) `buhk`
10. y - i (dirt) `dyrt`
11. yh - a (rat) `ryht`

### Voiced
12. j - g (collage) `kylahj`
13. l - l (lava) `lahva`
14. m - m (magma) `meigma`
15. n - n (neutral) `nutryl`
16. q - s (song) `soq`
17. r - r (render) `rendyr`
18. v - v (vortex) `vohrteks`
19. w - th (then) `wen`
20. z - z (zebra) `zibra`

### Unpitched
21. c - sh (shell) `cel`
22. f - f (fog) `fog`
23. h - h (have) `hyhv`
24. s - s (sing) `siq`
25. x - th (thick) `xihk`

### Plosive
26. b - b (base) `beis`
27. d - d (dance) `dyhns`
28. g - g (gas) `gyhs`
29. k - k (kelp) `kelp`
30. p - p (pretty) `prihti`
31. t - t (telepathy) `telepaxi`

### Combination Vowels
 - `au` (`ah` + `u`) - ow (cow) `kau`
 - `ai` (`ah` + `i`) - i (hi) `xai`
 - `eu` (`eh` + `u`) - ew (ew) `eu`
 - `ei` (`eh` + `i`) - ay (say) `sei`
 - `iu` (`ih` + `u`) - ew (ew) `iu`
 - `oi` (`oh` + `i`) - oy (boy) `boi`
 - `ui` (`uh` + `i`) - oy (doy) `dui`
 - `auu` (`a` + `u`) - ou (shout) `cauut`
 - `aii` (`a` + `i`) - ei (height) `xaiit`
 - `iuu` (`i` + `u`) - you (you) `iuu`
 - `uii` (`u` + `i`) - we (we) `uii`
