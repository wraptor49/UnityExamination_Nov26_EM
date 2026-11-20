COZY PIXEL FONTS LITE  (v1.3)
========================================
1 pixel font for cozy games, drawn pixel by pixel in code and exported as real TrueType and OpenType fonts plus BMFont bitmap fonts.
Free sample of Cozy Pixel Fonts (3 fonts).
- Cozy Pixel Tiny: native size 9px (use 9, 18, 27px...), cap height 5px, x-height 4px, 207 glyphs, proportional widths

CHARACTER SET (207 characters per font, see charset.txt)
- Full printable ASCII (U+0020 to U+007E): letters, digits and punctuation
- Full Latin-1 Supplement (U+00A0 to U+00FF): accented letters for French, Spanish, German, Portuguese,
  Italian and other Western European languages, plus symbols such as currency signs, guillemets and the degree sign
- Extras: Œ œ Ÿ € and typographic quotes, ellipsis, bullet, en and em dash, single guillemets

CONTENTS
- fonts/ttf/*.ttf and fonts/otf/*.otf   install on your computer or import in your engine
- bmfont/<font>/<font>_1x|2x|3x.fnt + .png   BMFont text format, white glyphs on transparent (tint in engine)
- glyph_sheets/*_glyphs_x4.png   every glyph with its code point
- charset.txt   all supported characters

KEEPING IT PIXEL PERFECT
The outlines are made of square pixels on a grid of 100 font units per pixel. Use the font at its native
size or a whole multiple of it, with antialiasing / smoothing turned off:
- Godot 4: import the .ttf, set Antialiasing to None, Hinting to None, Subpixel Positioning to Disabled,
  and use a font size that is a multiple of the native size. Or use the .fnt files directly.
- Unity: import the .ttf, set Rendering Mode to Hinted Raster (legacy Text) or create a TextMeshPro font
  asset with Render Mode RASTER and a sampling size equal to a multiple of the native size, Filter Mode Point.
- GameMaker, LOVE, MonoGame, Phaser and others that read BMFont: use the .fnt + .png for the scale you need.
There is no kerning; widths are proportional and each glyph includes 1px of spacing.

LICENSE (summary, see LICENSE.txt)
Free to use in personal and commercial projects (games, apps, videos, print), with or without credit.
Embedding is allowed: you may ship the font files inside your game or app builds, embed them in PDFs and
use them as web fonts for your project. Do not sell or redistribute the font files themselves,
do not register the fonts as a trademark, and do not use them to train AI models.

HOW THEY WERE MADE
Every glyph was drawn as a pixel grid in code (Python) and turned into fonts with fontTools. No AI image
generation was used.
