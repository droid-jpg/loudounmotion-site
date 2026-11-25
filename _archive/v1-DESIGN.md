---
name: Loudoun Motion
description: The web expression of the Loudoun Motion Brand, a Paper production script with one red record light.
colors:
  # Loudoun Motion Brand tokens. A base key holds the light-scheme value; its
  # "-dark-scheme" sibling replaces it under prefers-color-scheme: dark.
  # Tokens without a sibling are the same in both schemes.
  rec-red: "#E5322D"
  rec-red-text: "#CB1E19"
  rec-red-text-dark-scheme: "#FF6B66"
  surface: "#F4F1EA"
  surface-dark-scheme: "#18181B"
  surface-raised: "#FFFFFF"
  surface-raised-dark-scheme: "#232327"
  ink: "#18181B"
  ink-dark-scheme: "#F4F1EA"
  ink-muted: "#55555C"
  ink-muted-dark-scheme: "#A1A1AA"
  line: "#D6D3CB"
  line-dark-scheme: "#3F3F46"
  night: "#0A0A0B"
  on-night: "#F4F1EA"
  # Web-page extensions: derived in index.html, not in the brand tokens.
  ink-hover: "#34343A"
  ink-hover-dark-scheme: "#FFFFFF"
  on-night-muted: "#A1A1AA"
  night-raised: "#151518"
  night-control: "#74747C"
typography:
  display:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "clamp(2.75rem, 1.2rem + 5.4vw, 5.5rem)"
    fontWeight: 700
    lineHeight: 0.98
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "clamp(2rem, 1.4rem + 2vw, 2.5rem)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "-0.015em"
  lede:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "clamp(1.125rem, 1rem + 0.4vw, 1.3125rem)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
  small:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
    lineHeight: 1.55
  field-label:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 600
  button:
    fontFamily: "Inter Tight, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "-0.005em"
  readout:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "1rem"
    fontWeight: 500
    lineHeight: 1.3
    fontFeature: '"tnum"'
  timecode:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "0.8125rem"
    fontWeight: 500
    lineHeight: 1.85
    fontFeature: '"tnum"'
  label:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "0.75rem"
    fontWeight: 500
rounded:
  radius-none: "0px"
  radius-sm: "4px"
  radius-md: "8px"
spacing:
  space-1: "4px"
  space-2: "8px"
  space-4: "16px"
  space-6: "24px"
  space-8: "32px"    # web-page extension
  space-12: "48px"
  space-18: "72px"   # web-page extension
  space-24: "96px"   # web-page extension
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.surface}"
    typography: "{typography.button}"
    rounded: "{rounded.radius-sm}"
    padding: "0 24px"
    height: "48px"
  button-primary-hover:
    backgroundColor: "{colors.ink-hover}"
  button-compact:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.surface}"
    rounded: "{rounded.radius-sm}"
    padding: "0 16px"
    height: "40px"
  button-night:
    backgroundColor: "{colors.on-night}"
    textColor: "{colors.night}"
    rounded: "{rounded.radius-sm}"
    padding: "0 24px"
    height: "54px"
    width: "100%"
  button-night-hover:
    backgroundColor: "#FFFFFF"
  button-ghost-night:
    backgroundColor: "transparent"
    textColor: "{colors.on-night}"
    rounded: "{rounded.radius-sm}"
    padding: "0 24px"
    height: "44px"
  field-night:
    backgroundColor: "{colors.night-raised}"
    textColor: "{colors.on-night}"
    rounded: "{rounded.radius-sm}"
    padding: "14px 16px"
    height: "52px"
  segment-night:
    backgroundColor: "transparent"
    textColor: "{colors.on-night}"
    rounded: "{rounded.radius-sm}"
    padding: "0 8px"
    height: "48px"
  segment-night-selected:
    backgroundColor: "{colors.on-night}"
    textColor: "{colors.night}"
  nav-link:
    textColor: "{colors.ink}"
    padding: "4px 6px"
  record-light:
    backgroundColor: "{colors.night-control}"
    rounded: "50%"
    size: "10px"
  record-light-rolling:
    backgroundColor: "{colors.rec-red}"
  readout:
    backgroundColor: "{colors.night}"
    textColor: "{colors.on-night}"
    typography: "{typography.readout}"
    rounded: "{rounded.radius-sm}"
    padding: "10px 16px 10px 12px"
  timecode-gutter:
    textColor: "{colors.ink-muted}"
    typography: "{typography.timecode}"
    width: "8.25rem"
  script-beat:
    textColor: "{colors.ink}"
    padding: "24px 0"
  script-beat-live:
    backgroundColor: "{colors.surface-raised}"
  corner-guide:
    rounded: "{rounded.radius-none}"
    size: "22px"
  corner-guide-end-card:
    rounded: "{rounded.radius-none}"
    size: "40px"
  monitor:
    backgroundColor: "{colors.night}"
    textColor: "{colors.on-night}"
    rounded: "{rounded.radius-md}"
    width: "272px"
  monitor-progress:
    backgroundColor: "{colors.rec-red}"
    height: "6px"
  end-card:
    backgroundColor: "{colors.night}"
    textColor: "{colors.on-night}"
    padding: "48px 0 32px"
---

# Design System: Loudoun Motion

## Overview

**Creative North Star: "The Production Script"**

Every surface reads as a page of the script a spot is planned on. Paper is the sheet, ruled in hairlines; a timecode gutter runs down the left in JetBrains Mono; stage directions sit in a quieter Video column, and the words a viewer hears sit in the Audio column at full Ink. The camera shows up only through its instruments: one record light, a running timecode readout, a 9:16 monitor framed by viewfinder corner guides, and a Night end card that closes the page the way an ad closes. This file records the Loudoun Motion Brand design system as `index.html` implements it on the web, including the values the page had to add.

The density is a working document's: open rows, wide breaks between sections (96px), tight groups inside a row (8px), and nothing a script sheet would not carry. Hierarchy comes from Inter Tight's size and weight, from the step between Ink and Muted Ink, and from the 2px Ink rules that open a script and close a section head. Color does no hierarchy work. Red is spent on recording and nothing else, so when the light comes on it means something.

The result is technical and premium without costume: monospace only where a camera or a slate would print data, square corner guides only around something being framed, and flat, tonal depth. The brand book's confirmed rejections hold here too: no teal or any second accent, no gradients or glow, no hazard-style stripes, no underscore wordmark, no red dot in the corner of a tile.

**Key Characteristics:**
- A three-column production-script grid (timecode gutter, Video, Audio) is the layout grammar, ruled in hairlines rather than boxed.
- Ink on Paper in the light scheme, Paper on Ink in the dark; Night, fixed in both schemes, for everything on camera.
- One red: the record light, plus the monitor's progress bar.
- Inter Tight for everything people read; JetBrains Mono only for camera data.
- Flat: depth is tone, never shadow.
- Square viewfinder guides, 4px controls, an 8px video frame, and one circle: the record light.
- One ambient motion: the record light turns on and blinks. The sample spot plays only when asked.

## Colors

A script sheet and a camera: warm Paper and near-black Ink for reading, a deeper Night for anything on camera, and one red that means recording.

Each base token holds its light-scheme value; its `-dark-scheme` sibling replaces it under `prefers-color-scheme: dark`. The CSS custom property keeps the base name in both schemes, so components always reference the base token. Tokens marked *web-page extension* were derived on `index.html` and are not in the brand tokens.

### Primary
- **Record Light Red** (`rec-red`, #E5322D, both schemes): fills only. The dot in the mark, the hero readout's light while it rolls, the monitor's light while the spot plays, the steady REC light on the end card, and the monitor's progress bar. It is 3.9:1 on Paper, so it is never text.
- **Record Label Red** (`rec-red-text`, #CB1E19 light, #FF6B66 dark): the only red that may be text, for a small REC label or a highlight; 4.9:1 or better on Paper and Raised Sheet in both schemes. Declared on the page, not yet used.

### Neutral
Paper and Ink, which swap with the color scheme:
- **Paper** (`surface`, #F4F1EA light, #18181B dark): the page ground, and the label color of Ink buttons.
- **Raised Sheet** (`surface-raised`, #FFFFFF light, #232327 dark): the brand's ground for cards and panels on Paper. On this page it appears only as a state, the tint behind the live script row.
- **Ink** (`ink`, #18181B light, #F4F1EA dark): headlines, Audio-column copy, buttons, the 2px rules, focus rings and text selection; 15.7:1 on Paper.
- **Muted Ink** (`ink-muted`, #55555C light, #A1A1AA dark): stage directions in the Video column, timecode, column heads, section intros and notes; 6.5:1 or better on Paper and 6.1:1 or better on Raised Sheet, in both schemes.
- **Hairline** (`line`, #D6D3CB light, #3F3F46 dark): row dividers, the slug line's lower rule, the docked player's lower edge. Decorative only, never a control border.
- **Lifted Ink** (`ink-hover`, #34343A light, #FFFFFF dark; web-page extension): the Ink button's hover fill.

Night, the same in both schemes:
- **Night** (`night`, #0A0A0B): the camera's ground, under the hero readout, the monitor and the end card.
- **Paper on Night** (`on-night`, #F4F1EA): text, the reversed lockup, the Night button, the selected segment, focus rings on Night, and the corner guides at 42% (monitor) or 22% (end card) opacity; 17.5:1 on Night.
- **Dim Paper** (`on-night-muted`, #A1A1AA; web-page extension): STBY and other state words, format and shot descriptions, placeholders, form notes, the colophon; 7.7:1 on Night.
- **Night Field** (`night-raised`, #151518; web-page extension): the fill of text fields on Night.
- **Standby Gray** (`night-control`, #74747C; web-page extension): the idle record light and every control border on Night (fields, segments, the ghost button). It is 4.3:1 on Night: a control color, not a text color.

### Named Rules
**The Record Light Rule.** Red means recording. `rec-red` fills a record light or the spot's progress bar and nothing else: never a button, link, heading, border, background, error state or focus ring.

**The Ink Action Rule.** Every call to action is Ink on Paper, or Paper on Night inside the end card. Buttons are never red, so the light keeps its meaning.

**The Two Grounds Rule.** Paper is the script; Night is the camera. Anything shown as if on screen (the readout, the monitor, the end card) sits on Night, and Night does not change with the color scheme.

## Typography

**Display Font:** Inter Tight (with system-ui, sans-serif)
**Body Font:** Inter Tight (with system-ui, sans-serif)
**Label/Mono Font:** JetBrains Mono 500 (with ui-monospace, monospace)

**Character:** A tight, confident grotesk does all the reading, bold and close-set at display sizes; a mono appears only where a camera would print a readout. Both are self-hosted woff2 (Inter Tight as a 400–700 variable font in latin and latin-ext subsets, JetBrains Mono 500 in latin), with the latin files preloaded and `font-display: swap`.

### Hierarchy
The brand tokens fix a type scale for print and video; the web page runs its own fluid ramp. Each role notes how it relates to the brand token of the same name.

- **Display** (700, clamp(2.75rem, 1.2rem + 5.4vw, 5.5rem), so 44–88px; line-height 0.98; -0.035em; max 11ch, balanced): one per page, the first line of voiceover. The brand `display` token is 56px/56px; the web ramp passes it on viewports wider than about 680px and drops below it on phones.
- **Headline** (700, clamp(2rem, 1.4rem + 2vw, 2.5rem), so 32–40px; 1.05; -0.025em; max 22ch, balanced): section heads and the end-card heading. It tops out at exactly the brand `headline` (40px/42px).
- **Title** (700, 1.5rem; 1.25; -0.015em; balanced): step and question headings. Identical to the brand `title` (24px/30px).
- **Lede** (400, clamp(1.125rem, 1rem + 0.4vw, 1.3125rem), so 18–21px; 1.5; max 38ch): the offer under the headline. Web-page extension, no brand token.
- **Body** (400, 1.0625rem, so 17px; 1.55; 58–60ch max): script lines, step and answer copy. The brand `body` is 15px/22px; on the web it reads two pixels larger.
- **Small** (400, 0.9375rem, so 15px; 1.55): the slug line, navigation (at 500), on-screen super notes, form notes. Notes under the player and the colophon step down to 14px, and the script's column heads to 13px at 500. The brand `small` is 13px/18px.
- **Field label** (600, 0.9375rem): form labels and the fieldset legend. Step ordinals in the gutter use the same size and weight at line-height 1.9 to sit level with their title.
- **Button** (600, 1rem; line-height 1; -0.005em; never wraps): 15px on the compact header button, 17px on the Night button.
- **Readout** (JetBrains Mono 500, 1rem; 1.3; tabular numerals): the hero's record-light readout. The brand `readout` is 15px/20px.
- **Timecode** (JetBrains Mono 500, 0.8125rem, so 13px; 1.85; tabular numerals; Muted Ink): the script gutter. The tall line-height sets it roughly level with the first line of body copy beside it. Web-page extension.
- **Label** (JetBrains Mono 500, 0.75rem, so 12px): the monitor's HUD row. The same size as the brand `label` (12px/16px).

Inline mono (the email address, format specs) runs at 0.875em of its context with no tracking; the end-card URL is mono at 16px and the end card's top row mono at 14px.

### Named Rules
**The Camera Data Rule.** JetBrains Mono is for what a camera or a slate would print: timecode, REC, STBY and END, format specs (0:15 · 9:16 · 16:9), shot codes (ECU, MS, CU, WS), and the email address and URL. Never a headline, body copy, a label or a button.

**The Tabular Clock Rule.** Timecode is always HH:MM:SS:FF at 24 fps, in tabular numerals, so a running readout never jitters.

## Layout

The page is a 1280px maximum column with a fluid side margin of clamp(20px, 4vw, 48px). Its spatial model is the production script: an 8.25rem timecode gutter, then a Video column and an Audio column at 1fr to 1.65fr, 24px apart. Hero beats, steps and questions all sit on this grid; the sample script beside the monitor narrows the Audio column to 1.1fr. Section heads use the same gutter, leave it empty and start at the Video column.

Rhythm runs on the brand's 4px scale plus three page steps (32, 72 and 96px): 8px inside a group, 16px between a heading and its intro, 24px of padding in each script row (32px for steps and questions), 48px from the header to the first script, and 96px above each section and above the end card. The end card centres a 600px column with 72px above the lockup.

Measures stay readable: body copy 58–60ch, the lede 38ch, stage directions 34ch (46ch when stacked), the display headline 11ch.

Responsive behavior:
- **Up to 1100px:** the 272px monitor column (48px from the script, sticky 24px from the top) leaves the side of the sample script and docks above it as a strip: a 150px monitor beside a now-playing line, on Paper with a Hairline below, sticky at the top only while the spot plays.
- **Up to 860px:** the gutter collapses and every row stacks timecode, Video, Audio with 8px between; the column heads and the header's text links hide, leaving the compact button.
- **Up to 560px:** the lockup shrinks to 154px, the docked monitor to 112px with a compact HUD, and the end card's corner guides tighten to 24px at a 16px inset.

### Named Rules
**The Gutter Rule.** The left column holds a timecode, a step ordinal when order is the content, or nothing. Headings and copy always start at the Video column; a category label never sits above a heading.

**The Ruled Sheet Rule.** On Paper, structure is drawn with rules, not boxes: a 2px Ink rule opens a script and closes every section head, and 1px Hairlines divide the rows.

## Elevation & Depth

The system is flat. Nothing on the page casts a shadow; depth is tonal. Raised Sheet lifts the live script row off Paper, Night Field sets text fields into Night, and Night itself separates everything on camera from the script. In the dark scheme, where Night and the dark Paper sit close (1.1:1), the end card's top edge takes a 1px Hairline; the build draws it as `box-shadow: 0 -1px 0`, and it is a rule, not elevation. The brand's one shadow, a soft legibility shadow under the corner logo on footage, belongs to video and has no use on the page.

### Named Rules
**The Flat Sheet Rule.** Nothing is raised by a shadow. When something must stand apart, it changes ground: Paper to Raised Sheet, or Paper to Night.

## Shapes

Three radii and one circle. The mark and the viewfinder corner guides are square (`radius-none`): L-shaped 2px strokes with square ends, 22px on the monitor at a 14px inset (the lower pair 22px up, clear of the progress bar) and 40px on the end card at a 24px inset, in Paper at reduced opacity. Controls (buttons, fields, segments, the readout) take the 4px `radius-sm`. The video frame, the monitor, takes the 8px `radius-md`. The record light is the only circle. Bands are square: the live-row tint fills its row edge to edge, and the end card is full-bleed, so on the web it carries no radius where the brand gives print and video end cards `radius-md`. Rules are 1px Hairlines and 2px Ink. Focused links soften their outline to a 2px radius.

### Named Rules
**The Square Guide Rule.** Corner guides and the mark are never rounded, and a guide is always one of four L-shaped strokes at the four corners of what is being framed.

## Components

### Buttons
Ink blocks with a plain label: tactile, confident, never red.
- **Shape:** gently squared corners (4px, `radius-sm`); at least 48px tall with 24px side padding; an optional 14px authored SVG icon sits 8px before the label.
- **Primary:** Ink fill, Paper label in the button style. "Get a quote" and "Play the spot".
- **Hover / Active / Focus:** the fill eases to Lifted Ink over 0.2s; a press nudges it down 1px; keyboard focus draws a 2px Ink outline 3px out.
- **Compact:** 40px tall, 16px padding, 15px label. Only the header's "Get a quote".
- **Night:** on the end card the action inverts: Paper fill, Night label, full width, 54px tall, 17px label. Hover goes to pure white (#FFFFFF); focus is a Paper outline.
- **Ghost on Night:** transparent with a 1px Standby Gray border and a Paper label, 44px tall; hover turns the border Paper. Used for "Copy message".

### Inputs / Fields
Fields live only on Night, inside the end card.
- **Style:** Night Field fill, Paper text, 1px Standby Gray border, 4px corners, 52px minimum height (104px for the textarea, which resizes vertically), 14px by 16px padding, 16px text. Labels sit 8px above in the field-label style; "Optional" follows in Dim Paper at 400. Placeholders are Dim Paper.
- **Hover / Focus:** hover lifts the border to Dim Paper; focus turns it Paper and adds a 2px Paper outline 1px out.
- **Error:** never red. The border turns Paper and an inset 1px ring doubles it to 2px; below, a 15px Paper message that names the fix follows a 16px authored alert icon (a stroked circle with a bar and a dot).

### Segmented Choice
The ad-length picker: three equal options in a row, 8px apart, each 48px tall with a 1px Standby Gray border, 4px corners and a label at 500. Hover lifts the border to Dim Paper; the chosen option fills Paper with a Night label at 600; keyboard focus draws a 2px Paper outline 2px out. The native radio stays in place, invisible, over each option.

### Navigation
A single row 24px from the top. The lockup (186px by 34px; 154px by 28px up to 560px) links back to the top and swaps to the reversed lockup in the dark scheme. Text links are 15px at 500 with 4px by 6px padding and no underline until hover, when a 2px underline appears at a 0.22em offset. The compact Ink button ends the row. Up to 860px the text links hide and only the button remains. The header does not stick.

### Record Light and Readout
The page's one ambient motion. A 10px circle (12px inside the hero readout) rests in Standby Gray; when it starts rolling it eases to Record Light Red over 0.5s and blinks on a hard step, on for about 0.63s of each second and dimmed to 28% opacity for the rest. The hero readout is a Night pill (4px corners, 10px 16px 10px 12px padding, 8px gaps) holding the light, a Dim Paper state word (STBY, then REC) and a Paper timecode in the readout style. The light turns on 700ms after load, and the timecode rolls from 00:00:00:00 to 00:00:15:00 at 24 fps and loops. Under reduced motion it is lit from the start, does not blink, and reads 00:00:15:00. On the end card the light is steady red beside "REC".

### Production-Script Grid
The layout grammar as a component. A slug line opens it: a 2px Ink rule above, a Hairline below, 16px padding, the spot's name in 600 on the left and the format specs in Muted Ink mono on the right. Column heads (Timecode, Video, Audio) follow in sentence case at 13px, 500, Muted Ink, quieter than the script. Each beat is a row on the three-column grid with 24px of padding and a Hairline below: timecode in the gutter, the stage direction in Muted Ink in the Video column, and what is heard in Ink in the Audio column. Cue labels (SFX, VO, Music) are set in 600 inside the line; an on-screen super appears under its direction as "On screen:" in 15px Muted Ink with the quoted super in 600 Ink. The last beat, "Out.", drops its rule. On the hero, the Audio column carries the display headline, the lede and the actions.

### Sample Spot Monitor ("Play the spot")
A 9:16 Night frame, 272px wide, with 8px corners and four 22px corner guides in Paper at 42%. A HUD row 46px from the top carries the record light, the state (STBY, REC, END), the running timecode and the format (9:16) in the 12px mono label style; the format and then the state drop out as the frame narrows (container widths 230px and 170px). The current shot code (ECU, MS, CU, WS, END) sits centred at 41% of the height in 28px mono tracked +0.04em, with a 14px Dim Paper description below. The on-screen super rises 6px and fades in over 0.3s near the foot, in Inter Tight 700 at 20px, and a 6px progress bar fills along the bottom edge in Record Light Red over a dark track. The Ink "Play the spot" button below swaps its authored icon and label through Pause, Resume and Play it again. While the spot plays, the matching script row fades in a Raised Sheet tint across its full width (0.3s), its timecode and direction turn Ink, and it scrolls into view if it has dropped below the fold.

### Night End Card
The page closes the way a spot does. A full-bleed Night band 96px below the last section, framed by four 40px corner guides in Paper at 22% (24px at a 16px inset on phones). The top row, in 14px mono Dim Paper, carries the steady REC light and label on the left and 00:00:15:00 on the right. A centred 600px column holds the reversed lockup (up to 320px wide), the headline 48px below it, a Dim Paper intro, then the quote form. The URL follows in 16px mono and a 14px Dim Paper colophon closes the page. Inside the card, selection inverts to Paper and Night and focus rings turn Paper. A sent form reveals a status block under a Paper rule at 22% opacity, with the drafted email set in 15px sans in Dim Paper and a ghost "Copy message" button.

## Do's and Don'ts

### Do:
- **Do** make every call to action an Ink button on Paper (Lifted Ink on hover) or a Paper button on Night, with 4px corners and a target of at least 48px (40px only for the compact header button, 44px for a secondary control).
- **Do** set every timecode as HH:MM:SS:FF at 24 fps in JetBrains Mono 500 with tabular numerals.
- **Do** lay new sequenced content on the script grid: an 8.25rem gutter, then Video and Audio columns, rows divided by 1px Hairlines.
- **Do** keep stage directions in Muted Ink and what the viewer hears in Ink; a live row lifts both to Ink on a Raised Sheet tint.
- **Do** frame anything shown as if on screen with four square corner guides in Paper on Night: 42% opacity on the monitor, 22% on the end card.
- **Do** use the reversed lockup on Night and in the dark scheme, never narrower than 120px.
- **Do** theme the browser's own surfaces: selection inverts Ink and Paper (Paper and Night on the end card), the scrollbar is Muted Ink on Paper, links underline at 1px with a 0.22em offset and thicken to 2px on hover, and focus is a 2px outline 3px out in Ink (Paper on Night).
- **Do** let the record light carry the only ambient motion: it turns on once, then blinks on a hard one-second step; under reduced motion it stays lit and still.

### Don't:
- **Don't** set text in `rec-red`; when red must be text, use `rec-red-text`. Never make a button, link, heading, border, background, error or focus ring red.
- **Don't** add a second accent color (teal was tested and rejected), a gradient, a glow or hazard-style stripes.
- **Don't** set headlines, body copy, labels or buttons in JetBrains Mono.
- **Don't** park the record light alone in the corner of a tile or panel, where it reads as a notification badge.
- **Don't** use `line` for control borders; controls on Night take `night-control`, and `night-control` is never text.
- **Don't** raise anything with a shadow; change its ground instead.
- **Don't** put a category label or eyebrow above a heading; the gutter beside it holds a timecode, a step ordinal or nothing.
- **Don't** round the corner guides or the mark.
