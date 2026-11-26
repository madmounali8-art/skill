video-palettes

A Claude skill that holds ready-made color palettes and fonts for videos, reels, carousels, covers and thumbnails.

Whenever someone asks Claude to make a video or visual design, Claude asks which colors to use first, then applies the chosen palette and fonts consistently.

What's inside
Palette	Style
Neon Navy	Tech / programming, purple-blue-cyan gradient on dark navy
Coral & Black	Bold talking-head reels, coral highlight on black
Clean White Carousel	White slides with purple/blue/cyan accents
Coral & Gold on Navy	Warm accents on a navy background
Mint on Night Blue	Calm, glass-style look
Custom	Your own HEX colors

Fonts: Rubik (default, supports Arabic + Latin), JetBrains Mono (code), Inter (Latin), Tajawal + Noto Kufi (optional Arabic alternative).

Install

The skill is one file: SKILL.md.

Claude.ai
Put SKILL.md inside a folder named video-palettes.
Zip the folder.
Open Claude's settings, go to the Skills section, and upload the zip.
Claude Code

Copy the folder into your skills directory:

bash
# for all your projects
mkdir -p ~/.claude/skills
cp -r video-palettes ~/.claude/skills/

# or for one project only
mkdir -p .claude/skills
cp -r video-palettes .claude/skills/
How to use

Just ask Claude for a video or design. You don't need to mention the skill.

Example:

You: Make me a 9:16 intro video for my coding channel.

Claude: Which colors would you like? Neon Navy, Coral & Black, Mint on Night Blue, or your own colors?

You: Neon Navy.

Claude: Done, using Neon Navy with Rubik. Starting now.

Skip the question by naming the palette up front:

Make a carousel about CSS Grid using the Coral & Black palette.

Or give your own colors:

Make a thumbnail with background #101820 and accent #FEE715.

Customize

Open SKILL.md and edit the palette tables. To add a palette, copy one table, rename it, and change the HEX values. Keep the rule that Claude asks before starting.

Rules built into the skill
Claude asks one question about colors before starting, unless you already named them.
One palette per video, no mixing.
No extra colors or fonts unless you ask.
Captions are large, high contrast, with one highlighted word per line at most.
Arabic text is right-to-left.
Sizes: video 9:16, carousel 1080×1350 (4:5).
License

MIT. Rubik, JetBrains Mono, Inter, Tajawal and Noto Kufi are open-source fonts (OFL).
