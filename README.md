# Deskcress 1.0 TEST
Native Android Desk Place straight-triomino exact-cover puzzle. Android 8+ (min26), target35. Package com.gg007.deskcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Desk Place / Wittgenstein Briquet training puzzle on a 4x4 grid. Tap unnumbered cells to shade or clear them. The dark cells must be exactly tileable by nonoverlapping straight 1x3 desks, horizontal or vertical. Desks MAY touch each other. Numbered cells stay light; each number counts side-adjacent dark cells, not diagonals. All light cells, including clues, must form one edge-connected floor. No total desk count is given. Automatic gold outlines show one valid desk partition when the current shading is tileable. Outlines do not impose a separate player-drawn partition. Twelve original uniquely solvable shadings; auto-check after every tap, unlimited undo/reset, next and level selection. Saved palette and optional dots repeat occupied desk cells. Unshaded cells may remain blank; no explicit light notes, timer or ranking.

## Download and status
https://mega.co.nz/#!0QFiQYZY!Y-d-csKn3MB5Zf2Qel49T4NzG_0lu9K2OrFjD1P3r9A
APK SHA256 a5112baae13516ab144e42454f1f3e52932d88f0ee45dcdfa8131d585cf175b2; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent all-subset enumeration of sixteen geometric 1x3 placements plus set-based flood fill versus production lowest-bit recursive exact cover and growing-bitset connectivity passed 786,432 complete shade masks, all 65,536 masks on each of twelve boards, plus 65,536 tiling/connectivity/cover comparisons. Each board has exactly one full-rule shading; a shading may have more than one block partition, which is accepted. Tests cover touching desks, bent or incomplete shape rejection, disconnected light floor, clue lock, invalid bounds, automatic cover extraction, undo, solved lock, reset and replay. Portable generator with seed 500209 reproduces all twelve boards; archived Java oracle reruns. Actual drawing-adapter cell taps, solve/undo/replay, next, levels, menu, privacy and saved palette/desk-cell settings pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 181 prior studio descriptions and web registry game/mechanic records. Statuefern places separated L and T shapes from a bank; Gazefen shades separated squares with sight restrictions; Brickcress shades staggered bricks with downward support and a horizontal run limit. Deskcress instead permits touching straight triomino desks, validates an exact cover of the dark shading, matches local side-neighbor counts and connects the light complement. Its cover recursion and complement-connectivity validator differ from those games. No Desk Place match found in the reviewed corpus; recovered repository corpus remains partial. Known Desk Place / Wittgenstein Briquet adaptation, not a global invention claim. Original generated boards, code and visuals; no source puzzle layouts, code or art copied.
Rules https://puzzlecake.blogspot.com/p/wittgenstein-briquet-rules.html ; independent rules https://dj-puzzles.blogspot.com/2025/04/genre-spotlight-29-desk-place-puzzles.html .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/deskcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.deskcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Deskcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, desk cell marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 182-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/aub8k0bxf9sc-deskcress-source-archive . Repository https://github.com/iLanis-agent/deskcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
