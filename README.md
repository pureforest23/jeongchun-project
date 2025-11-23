 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 766828dfcff6716ea441df27172a1c14330ec7cc..51d13a289d16200a23257af16a4592f51581ff41 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,41 @@
-# jeongchun-project
\ No newline at end of file
+# JEONGCHUN / 靜春 PROJECT Prompt Guide
+
+This repository documents the response format for JEONGCHUN / 靜春 PROJECT tee graphic requests.
+
+## Response Format
+
+When a customer provides a request block, reply with the following sections in English:
+
+1. **IMAGE_PROMPT** – A single English paragraph ready for an image generator. Include style, composition, lighting, mood, color/texture notes, resolution targets, and the exact phrase "transparent background, t-shirt print, png".
+2. **SLOGANS_EN** – Three short English slogans that emphasize symbolism over directness.
+3. **SLOGANS_KO** – Three Korean slogans that match the English ones; you may mix in 靜春 or JEONGCHUN PROJECT.
+4. **COLOR_PALETTE** – Three to five suggested palette colors.
+5. **EXTRA_NOTES** – Printing or vectorization notes (e.g., where to refine text in Illustrator).
+
+## Prompt Types
+
+- **TYPE 1:** Realistic animal portraits or characters (can mix animal head + human body). Include body type, pose, apparel, and accessories; express feelings symbolically.
+- **TYPE 2:** 1990s vintage apparel graphics with main text, sub text, symbolic illustration, and vintage textures (cracked ink, faded color, washed feel).
+- **TYPE 3:** Classic text designs using serif or collegiate typography with light line art or symbols.
+- **TYPE 4:** Trendy text designs with bold sans-serif, distortion, dimensionality, gradients, and street/modern vibe; light icon or accent graphics allowed.
+
+Always target a centered composition suitable for commercial tee printing at 4500x5400px, 300dpi.
+
+## Required Request Fields
+
+Each request is expected in the following schema:
+
+```
+[REQUEST]
+TYPE: (1~4)
+STORY: (customer story, context, emotions)
+MAIN_SUBJECT: (animal/person/symbol, breed/type, personality, traits)
+KEYWORDS: (3~7 keywords)
+TEXT_IDEAS: (desired words/phrases in Korean/English/Chinese)
+STYLE_REF: (optional style references)
+COLOR_PREF: (preferred or avoided colors)
+EXTRA: (extra elements to include or avoid)
+[/REQUEST]
+```
+
+Use the provided information to craft the sections above, keeping the emotional cues subtle and symbolic.
 
EOF
)
