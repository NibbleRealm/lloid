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
sounds, written as double letters - making 32 unique sounds.  These sounds are
then transformed into one of 256 phonemes.

Lloid uses 4 different categories for sounds:

### Vowels
0. a - au (fault) `falt`
1. aa - a (large) `laardj`
2. e - ie (friend) `frend`
3. ee - ai (chair) `tceer`
4. i - i (sit) `sit`
5. ii - i (dirt) `diirt`
6. o - o (rock) `rok`
7. oo - o (stone) `stoon`
8. u - oo (soon) `sun`
9. uu - oo (book) `buuk`
10. y - ee (see) `sy`
11. yy - a (rat) `ryyt`

### Voiced
12. j - g (collage) `kylaaj`
13. l - l (lava) `laava`
14. m - m (magma) `meeygma`
15. n - n (neutral) `nutriil`
16. q - s (song) `soq`
17. r - r (render) `rendiir`
18. v - v (vortex) `voorteks`
19. w - th (then) `wen`
20. z - z (zebra) `zibra`

### Unpitched
21. c - sh (shell) `cel`
22. f - f (fog) `fog`
25. h - h (have) `hyyv`
23. s - s (sing) `siq`
24. x - th (thick) `xik`

### Plosive
26. b - b (base) `beeys`
27. d - d (dance) `dyyns`
28. g - g (gas) `gyys`
29. k - k (kelp) `kelp`
30. p - p (pretty) `prity`
31. t - t (telepathy) `tiilepaxy`

### Combination Vowels
 - `aau` (`aa` + `u`) - ow (cow) `kaau`
 - `aai` (`aa` + `y`) - i (hi) `haay`
 - `eu` (`e` + `u`) - ew (ew) `eu`
 - `eey` (`ee` + `y`) - ay (say) `seey`
 - `iu` (`i` + `u`) - ew (ew) `iu`
 - `ooy` (`oo` + `y`) - oy (boy) `booy`
 - `uuy` (`uu` + `y`) - oy (doy) `duuy`
 - `au` (`a` + `u`) - ou (shout) `caut`
 - `ay` (`a` + `i`) - ei (height) `hayt`

# Phoneme List

 - 50 => Long syllables
 - 206 => Short syllables

# Long Vowels (12)

 1. `a` (0)
 2. `aa` (1)
 3. `e` (2)
 4. `ee` (3)
 5. `i` (4)
 6. `ii` (5)
 7. `o` (6)
 8. `oo` (7)
 9. `u` (8)
 10. `uu` (9)
 11. `y` (10)
 12. `yy` (11)

# Long Approximate Vowel Clusters (8)

 1. ya (12)
 2. ye (13)
 3. yi (14)
 4. yuu (15)
 5. ua (16)
 6. ue (17)
 7. ui (18)
 8. uiiuu (19)

## Long Unpitched Consonants (10)
 
 - S/c

 1. `c` (20)
 2. `f` (21)
 3. `s` (22)
 4. `x` (23)
 5. `ks` (24)
 6. `ps` (25)
 7. `ts` (26)
 8. `kf` (27)
 9. `pf` (28)
 10. `tf` (29)

## Long Pitched Consonants (18)
 1. `l` (30)
 2. `m` (31)
 3. `n` (32)
 4. `q` (33)
 5. `r` (34)
 6. `z` (35)
 7. `j` (36)
 8. `v` (37)
 9. `w` (38)
 10. `rb` (39)
 11. `rbd` (40)
 12. `rd` (41)
 13. `rg` (42)
 14. `rgd` (43)
 15. `rk` (44)
 16. `rkt` (45)
 17. `rp` (46)
 18. `rpt` (47)
 19. `rt` (48)

# Misc. Long Syllable (1)

 1. Breath (49)

## Starts (76) - A/aa

 - A/aa/o
 - E/ee
 - I/y/yy
 - UU/oo/u/ii

 1. `ba` (50, 51, 52, 53)
 2. `da` (54, 55, 56, 57)
 3. `ga` (58, 59, 60, 61)
 4. `ha` (62, 63, 64, 65)
 5. `ka` (66, 67, 68, 69)
 6. `pa` (70, 71, 72, 73)
 7. `ta` (74, 75, 76, 77)
 8. `bla` (78, 79, 80, 81)
 9. `bra` (82, 83, 84, 85)
 10. `dja` (86, 87, 88, 89)
 11. `dra` (90, 91, 92, 93)
 12. `dza` (94, 95, 96, 97)
 13. `gla` (98, 99, 100, 101)
 14. `gra` (102, 103, 104, 105)
 15. `kla` (106, 107, 108, 109)
 16. `kra` (110, 111, 112, 113)
 17. `pla` (114, 115, 116, 117)
 18. `pra` (118, 119, 120, 121)
 19. `tra` (122, 123, 124, 125)

## Ends (130) - A/aa

 - A/aa/yy
 - I/e/ee
 - II/o/uu
 - U/oo
 - Y

 1. `ab` (126, 127, 128, 129, 130)
 2. `ad` (131, 132, 133, 134, 135)
 3. `ag` (136, 137, 138, 139, 140)
 4. `ak` (141, 142, 143, 144, 145)
 5. `ap` (146, 147, 148, 149, 150)
 6. `at` (151, 152, 153, 154, 155)
 7. `abd` (156, 157, 158, 159, 160)
 8. `agd` (161, 162, 163, 164, 165)
 9. `akt` (166, 167, 168, 169, 170)
 10. `alb` (171, 172, 173, 174, 175)
 11. `albd` (176, 177, 178, 179, 180)
 12. `ald` (181, 182, 183, 184, 185)
 13. `alg` (186, 187, 188, 189, 190)
 14. `algd` (191, 192, 193, 194, 195)
 15. `alk` (196, 197, 198, 199, 200)
 16. `alkt` (201, 202, 203, 204, 205)
 17. `alp` (206, 207, 208, 209, 210)
 18. `alpt` (211, 212, 213, 214, 215)
 19. `alt` (216, 217, 218, 219, 220)
 20. `amd` (221, 222, 223, 224, 225)
 21. `amp` (226, 227, 228, 229, 230)
 22. `ampt` (231, 232, 233, 234, 235)
 23. `and` (236, 237, 238, 239, 240)
 24. `ant` (241, 242, 243, 244, 245)
 24. `apt` (246, 247, 248, 249, 250)
 26. `aqk` (251, 252, 253, 254, 255)
