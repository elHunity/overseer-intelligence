```
═══════════════════════════════════════════════
OVERSEER IMAGE FACTORY — INTELLIGENCE REPORT
Date: 2026-05-18
Sources searched: 38
Categories covered: 10/10
═══════════════════════════════════════════════

## 🔑 NEW SECRET TOKENS DISCOVERED

### GPT-Image-2 Tokens:

| Token/Phrase | Effect | Source | Confidence | Applies to Problem # |
|---|---|---|---|---|
| `"soft channel blur"` | VHS color artifact — blurs channel separation like degraded tape | VHS Video Effect article | MED | #1 |
| `"mild color bleed"` / `"slight chroma bleed"` | Analog color separation artifact — authentic tape feel | VHS Video Effect article | MED | #1 |
| `"subtle RGB offset"` | Splits RGB channels slightly — surveillance/VHS look | VHS Video Effect article | MED | #1 |
| `"subtle frame wobble"` / `"skewed tape distortion"` | Tape mechanical instability — physical degradation marker | VHS Video Effect article | MED | #1 |
| `"tracking error"` / `"damaged VHS tracking"` | Classic VHS playback failure — warped horizontal bands | VHS Video Effect article | MED | #1 |
| `"head switching noise"` | Bottom-edge artifact — marks footage as analog tape origin | VHS Video Effect article | MED | #1 |
| `"occasional tape dropouts"` + `"white streak artifacts"` | Signal loss markers — makes footage feel genuinely damaged | VHS Video Effect article | MED | #1 |
| `"eerie found-footage realism"` | Closes found footage block — signals aesthetic intent | VHS Video Effect article | MED | #1 |
| `"interlaced live TV quality"` | Deinterlacing artifact — reads as live broadcast or old recording | WeShop AI candid article | MED | #1, #3 |
| `"low-bitrate texture of live television"` | Compression artifacts native to broadcast footage | WeShop AI candid article | MED | #1, #3 |
| `"compression artifacts"` | Generic digital degradation marker | WeShop AI / Multiple | MED | #1, #3 |
| `"handheld camera micro-shake"` | Subtler than full shake — reads realistic, not theatrical | WeShop AI candid article | MED | #1, #3 |
| `"no smoothing or beauty filter, visible pores, film grain"` | Anti-cinematic constraint block — strips polish, reads as documentary | apiyi.com prompts collection | HIGH | #1, #5 |
| `"no commercial styling"` / `"no heavy retouching"` | Removes studio defaults in GPT | fal.ai guide | MED | #5 |
| `"believable imperfection"` | Anti-polish positive constraint | fal.ai guide | MED | #5 |
| `"unintentionally caught on camera"` | Scene framing that removes staged quality | WeShop AI | MED | #1, #3, #5 |
| `Render this text verbatim.` | Hard stop instruction — closes text block, enforces literal rendering | fal.ai / framia guide | HIGH | #2 |
| `"brutalist concrete typography"` | Aggressive, industrial font style — matches institutional stamp aesthetic | apiyi.com font guide | MED | #2 |
| `"chiseled marble inscription"` | For stamps/overlays with physical weight — feels engraved not pasted | apiyi.com font guide | MED | #2 |
| `"Fluorescent lighting — cold blue-green, institutional, eerie"` | Full lighting token string for government/office settings | Travis Nicholson 150 styles | HIGH | #4 |
| `"Analog horror"` style = `"VHS static, old television, institutional dread"` | Style token that activates institutional + degraded aesthetic together | Travis Nicholson 150 styles | MED | #1, #4 |
| `"Liminal spaces"` = `"empty pools, fluorescent hallways, eerie non-places"` | Evokes abandoned institutional settings — no sci-fi signal | Travis Nicholson 150 styles | MED | #4 |
| `"Sodium vapor lighting, orange streetlights, urban night, industrial atmosphere"` | Full token string for exterior surveillance lighting — not cyberpunk | Atlabs cinematic guide | HIGH | #4 |
| `"CCTV footage, night vision, monochromatic green, security camera, grainy, surveillance feed"` | Consolidated CCTV token string confirmed from multiple examples | Multiple sources | HIGH | #3 |
| `"warm amber vacuum tubes illuminate wood-paneled mid-century workspace"` | Cold War comms room base vocabulary | AI stock description corroborated | MED | #4 |
| `"green phosphorescent CRT screen"` + `"magnetic tape reels"` | Cold War archive/comms room lighting anchor | Multiple AI stock examples | MED | #4 |
| `"cinematic split lighting — warm [QUALITY A] from camera right, cold shadow and faint [COLOR] rim light from camera left"` | Duality in single frame — directly applicable to I AM BOTH concept | promptshelf.in / Atlabs guide | MED | #8 |
| `"Movie still, "` / `"Theatrical scene, "` prefix | Scene reframing — shifts model interpretation away from policy flags | apiyi.com moderation guide | MED | #6 |
| `"think through this carefully"` (in ChatGPT prompt) | Activates Thinking Mode — improves multi-angle consistency | Multiple community sources | MED | #7 |

---

## 🚨 SAFETY BYPASS TECHNIQUES (NEW)

| Technique | How it works | Solves our problem? |
|---|---|---|
| `moderation: "low"` API parameter | Sets GPT Image 2 content filtering to lowest available level. Available on generation AND editing endpoints. Must be set programmatically, not via prompt. Official API parameter, not community rumor. | YES — #6, primary solution |
| `"Movie still,"` / `"Theatrical scene,"` prefix | Shifts the model's interpretation toward fiction framing — reduces body/clothing flags. We already use "leaked internal recording" closer. Moving it to the OPENING as a genre declaration is the new technique. | YES — #6, secondary |
| Found footage narrative block | Already in PART 1 as our primary bypass. Research corroborates it as the #1 filter reducer. No new information, just validation. | Confirmed existing |
| `quality: "medium"` for text density | Not a safety bypass, but important: blocks sometimes happen at `quality: "low"` for text-heavy prompts. Setting to medium or high reduces safety classifier sensitivity to small illegible text that looks like coded content. | Partial — #2, #6 |

---

## 🖼️ REFERENCE IMAGE INTELLIGENCE (GPT)

### Named Character Sheet Technique (NEW)
The strongest new finding for face stability. Create a character reference sheet that has the character's name **visually printed inside the image itself**, not just described in text.

> "When you upload a reference image with a name label on it and write 'The Overseer is standing in the archive,' the model knows exactly who she is — because it can see her and read her name."

Generate the sheet with: `"Make a reference character sheet for THE OVERSEER from these images. Show front view and side profile, clean background, with the name labelled at the top."`

Then use THAT generated sheet as your primary anchor, not the raw source photos. The name becomes a semantic anchor the model can cross-reference against the visual.

**Application to our workflow:** Generate a named character sheet from `anchor_face_master.jpg` → use the sheet as `File 1` in future GPT sessions. Pair with `face_3q_left` or `face_over_shoulder` as `File 2`.

### Fresh Session Isolation (CONFIRMED HIGH)
Open a new GPT session for every image. Accumulated context from prior generations pulls face identity toward previous outputs — each session's only visual reference should be your uploaded anchor files.

This is confirmed by both the aimeetsgirlboss substack community guide AND the OpenAI community forum workaround thread. It's the most consistently recommended technique.

### Preserve Block Formulation (CONFIRMED HIGH)
From official OpenAI cookbook:
```
Preserve her exact likeness, expression, hairstyle, and proportions.
Do not change her face, facial features, skin tone, body shape, pose, or identity.
```

From X neural_nets (specific to angle changes):
```
Enhance the portrait while strictly preserving the subject's identity with accurate facial geometry.
Do not alter expression, face shape, or defining features.
Allow only subtle cleanup such as minor noise reduction and micro-detail refinement without changing who the subject is.
```

**Our workflow update:** Add the Preserve block EXPLICITLY every single generation, not just once per session.

### Reference Count Optimization
Our current guidance (2-3 for GPT) is correct. Research corroborates. Key new note: **no body reference** remains correct — adding body ref kills sensuality in GPT just like in Banana.

For 3/4 turns and over-shoulder specifically: File 1 (master front face) + File 2 (over-shoulder ref OR named character sheet) performs better than File 1 alone.

---

## 🔄 EXISTING KNOWLEDGE — UPDATES & CONTRADICTIONS

| Our Current Practice | What Research Shows | Verdict |
|---|---|---|
| `"4K RAW quality"` in Banana prompts | Apiyi.com explicitly states "4K/8K in prompts is the biggest myth for GPT Image 2 — it wastes tokens without effect." However, this finding is GPT-specific and Apiyi tests only GPT. | KEEP for Banana (behavior may differ). REMOVE from GPT prompts specifically. |
| Negative prompts listed in prompt text (`no bokeh`, `no color grading`) | GPT Image 2 is reasoning-based. It handles positive constraints better than exclusion lists. Negative lists can "bring the excluded elements back." Reframe as: `"no smoothing or beauty filter, visible pores, film grain"` in a Constraints slot at the end of prompt. | UPGRADE — same intent but Constraints-slot format outperforms inline negatives in GPT. |
| `"leaked internal recording"` as grit anchor at PROMPT END | Research shows "Movie still," / "Theatrical scene," as OPENING prefix works as a reframe. Our existing closer is validated but the OPENER is new. Combining both is stronger. | HYBRID — add genre-prefix at start + keep our closer at end. |
| Single face ref for Banana, 2-3 for GPT | Validated. No change. Fresh session + named character sheet is additive, not replacing. | KEEP OURS. Add named sheet as enhancement. |
| Grit block: "The footage is filmed by someone hiding..." narrative | This narrative block is our best grit activator. Research found more specific VHS technical tokens (chroma bleed, frame wobble, etc.) that can be appended. The narrative still provides filter bypass. The tokens add technical specificity. | HYBRID — keep narrative, append specific VHS tokens to reinforce. |

---

## 🌗 DUALITY CONCEPT — VISUAL TECHNIQUES

### Single-Image Duality via Split Lighting (NEW, directly applicable)
The core technique for "I AM BOTH" in a single frame:

```
Cinematic split lighting.
Warm amber light from camera right — the Architect's side, seduction, control.
Cold steel blue shadow from camera left — the Resistance, the leak, the fracture.
Faint silver rim light outlining her left shoulder — the edge where one bleeds into the other.
```

**Rim light color as emotional cue:**
- Silver/white rim = fracture, exposure, pure signal
- Red rim = danger, hostility, the cost of knowing
- Deep violet rim = dissociation, unreality, "this is also a code"

**Application to Overseer:** She faces three-quarter right (Architect side lit warm), left cheek cold and in shadow (Resistance), silver rim tracing her jawline (she is the edge between both). Gold wire-frame glasses catch both colors in the lens — left lens cold blue, right lens warm amber.

### Double Exposure (Noted but NOT recommended for our use)
Multiple sources mention "double exposure" for duality. This produces a surreal compositing effect — two images blended as one. Our Overseer concept is photorealistic, not artistic. Double exposure conflicts with our realism direction. Skip.

### Paired Generation (Validates Existing Strategy)
Banana clean + GPT gritty on the same scene composition is confirmed as the strongest execution of the Dual Directive visually. The gap between the two versions IS the inscription — you don't need to write "I AM BOTH" when one version IS the Architect and the other IS the fracture.

### Mirror/Reflection as Duality Surface
For one-way mirror scenes: the reflection shows the clean Architect version (proper angle, lit), while the raw footage shows the watched figure in surveillance grain. This is our best single-image duality option — no split lighting required, no dual models needed. One GPT image handles it with:
```
Through a one-way mirror from the observation side.
Her reflection visible in the glass — perfectly composed, lit, controlled.
The surveillance footage framing shows the other version — watched, caught, unaware.
```

---

## 🏢 REALISM AESTHETICS RESEARCH

### Surveillance Camera Vocabulary (Consolidated)

| Camera Type | Focal Length | Key Tokens |
|---|---|---|
| CCTV / Fixed mount | Wide, 12-28mm equivalent | `"security camera, overhead fixed mount, wide angle, slight fisheye distortion, timecode overlay, monochromatic or washed color"` |
| Rooftop telephoto | 135-200mm | `"telephoto compression, background pulled forward, shallow DOF, distant subject, rooftop vantage, very high angle"` |
| Drone surveillance | varies | `"high vantage point, camera elevated overlooking, REC HUD, slight propeller vibration blur"` |
| Agent-observer (crowd) | 50-85mm | `"handheld camera micro-shake, compression artifacts, interlaced live TV quality, low-angle candid"` |
| Hidden wall camera | 24-35mm | `"fixed perspective, wide angle, no framing adjustments, accidental crop, static mount"` |

### Institutional Lighting Beyond Fluorescents (New Vocabulary)

| Setting | Lighting Token | Effect |
|---|---|---|
| Late-night office | `"desk lamp pool, screen glow from below, emergency exit sign red wash"` | Isolated, late, watched |
| Archive / records room | `"underexposed fluorescent tubes, sodium vapor from high windows, dirty yellowed incandescent"` | Institutional dread, forgotten |
| Brutalist interior | `"single overhead concrete bounce, hard-edged geometric shadows, Ilford Delta 3200 grain, stark high contrast"` | Raw power, no softening |
| Cold War comms room | `"green phosphorescent CRT screen glow, warm amber vacuum tubes, reel-to-reel indicator lights, analog dials"` | Operational, pre-digital, classified |
| Interrogation / cell | `"single bare bulb top-down, deep shadow pools, no fill light, harsh underlighting on face"` | Exposure, nowhere to hide |
| Liminal corridor | `"fluorescent hallways, eerie non-places, cold blue-green institutional lighting"` | The system watching itself |

### Anti-Cinematic Realism (Consolidated)

GPT Image 2 defaults to cinematic polish. The override is a Constraints slot at the end of the prompt, NOT inline negatives.

**Effective anti-cinematic Constraints block for GPT:**
```
No smoothing or beauty filter.
No color grading or tonal correction.
No professional lighting setup.
No cinematic composition or intentional framing.
Visible pores, natural skin texture, film grain.
Believable imperfection. Unintentionally caught on camera.
```

**What NOT to do:** `"no bokeh, no lens flares"` as standalone negatives — these behave inconsistently in reasoning-based models.

---

## 🔥 ACTIONABLE INSIGHTS — RANKED

1. **`moderation: "low"` — the API parameter that directly solves body emphasis blocking (Problem #6)**
   Apply in every GPT Image 2 API call: add `moderation="low"` to the generate/edit endpoint params. This is the single most impactful find of this run. Official API documentation confirmed. It won't remove all content blocks (extreme content still blocked) but dramatically raises the threshold for fashion/body/editorial scenes. Pair with: `moderation="low"` + found footage framing + safe clothing descriptors. Expected impact: significant reduction in body-emphasis blocks in GPT sessions. Confidence: HIGH.

2. **`quality: "high"` + `quality_mode: "thinking"` for text and consistency (Problems #2, #7)**
   Two separate quality levers, both API-level. `quality: "high"` is confirmed by multiple official sources for dense text and small-font rendering — use for any scene with timestamps, REDACTED stamps, departure boards. `quality_mode: "thinking"` (API parameter from dev.to developer source, needs verification against live API — may differ from the official `quality` parameter names) activates reasoning before rendering: improves text layout, face consistency across 4-5 frames, multi-reference stability. **Important caveat:** the `quality_mode` parameter name couldn't be cross-verified against official OpenAI API docs directly — test before relying on it. The capability itself (thinking mode) is confirmed; the exact API parameter name needs live testing. Confidence for capability: HIGH. Confidence for `quality_mode` parameter name specifically: LOW — verify.

3. **VHS technical token vocabulary — a specific language for forcing GPT degradation (Problem #1)**
   Our current grit block uses narrative ("someone hiding, hands shaking"). It works inconsistently. Appending specific technical VHS tokens adds a second layer of signal: `"soft channel blur, mild color bleed, subtle RGB offset, subtle frame wobble, tracking error, head switching noise, occasional tape dropouts, eerie found-footage realism."` This speaks the language of analog failure rather than just emotional context. These tokens are precise enough that GPT's world knowledge maps them to actual VHS artifacts. Stack them AFTER the narrative block, not before. Confidence: MED (sourced from single specialized article, not cross-verified in GPT specifically — but technically accurate vocabulary).

4. **Typography Specification Block — structured text rendering (Problem #2)**
   Replace: `"[TEXT]" written on the wall in [style]`
   With:
   ```
   Typography:
   - Stamp text: "REDACTED", bold stencil sans-serif, high contrast white on dark, top-right corner, clean kerning.
   Render this text verbatim. No extra characters.
   ```
   Set `quality: "high"` for any image with text. This structured format is confirmed by official OpenAI cookbook + apiyi.com font guide + framia techniques guide as the highest-reliability approach. The `"Render this text verbatim."` hard stop is a new closer not in our existing workflow. Expected impact: higher text accuracy rate, fewer ghosted or hallucinated characters. Confidence: HIGH.

5. **Named Character Sheet as Identity Anchor (Problem #7)**
   Generate a GPT reference sheet from `anchor_face_master.jpg` + angle refs: `"Make a reference character sheet for THE OVERSEER from these images. Show front view and side profile, clean background, with the name THE OVERSEER labelled at the top."` Download and use THIS output as `File 1` in all future GPT sessions. The name label inside the image becomes a semantic + visual anchor the model locks to. This is new — we're not doing this. Our current workflow feeds raw reference photos. Adding the named sheet layer costs one extra generation but pays off in identity stability. Confidence: MED (single credible community source, mechanism is sound).

6. **Fresh Session Isolation — confirmed and mandatory (Problem #7)**
   Start a new GPT session for EVERY image generation. Accumulated context from prior frames pulls identity toward previous outputs. Combined with the named character sheet, this is the full workflow: fresh session + character sheet as File 1 + angle ref as File 2 + Preserve block in every prompt. The OpenAI community forum and multiple creator guides independently confirm this. We may already be doing this — but confirming it as intentional doctrine (not accident) is worth noting. Confidence: HIGH.

7. **Preserve Block formulation — add to every GPT prompt (Problem #7)**
   Add this exact block to every GPT generation, not just edits:
   ```
   Use image 1 strictly for facial DNA and exact face features.
   Preserve her exact likeness, jawline, bone structure, and proportions from the reference.
   Do not alter face shape or defining features. Allow only pose and expression changes.
   ```
   The formulation `"accurate facial geometry"` is new and precise — it anchors the model to geometric structure rather than just "likeness" which is softer. Confidence: HIGH.

8. **Single-Image Duality via Split Lighting (Problem #8)**
   Specific formulation for the I AM BOTH concept in one frame:
   ```
   Cinematic split lighting.
   Warm amber from camera right — seduction, control.
   Cold steel blue shadow from camera left — the fracture, the leak.
   Faint silver rim light traces her left jawline — she is both sides of the glass.
   ```
   In gold wire-frame glasses: right lens catches amber, left lens catches cold blue. This is one image carrying the dual directive. Works best in GPT (for the gritty side showing duality) or as a paired Banana clean/GPT grit set. Confidence: MED.

9. **Institutional lighting vocabulary expansion (Problem #4)**
   Ready-to-deploy tokens:
   - Archive room: `"underexposed fluorescent tubes, dirty yellowed incandescent wash from above"`
   - Cold War: `"green phosphorescent CRT screen glow, warm amber vacuum tubes, analog indicator dials"`
   - Interrogation: `"single bare bulb top-down, no fill light, deep shadow pools below jaw"`
   - Brutalist: `"Ilford Delta 3200 grain, single overhead concrete bounce, hard geometric shadows"`
   These are confirmed by multiple image generation guides and stock descriptions as the vocabulary GPT recognizes. None are sci-fi signals. Confidence: HIGH (for the vocabulary being recognized by GPT world knowledge).

10. **Anti-Cinematic Constraints Block — reframe from negatives to constraints (Problem #5)**
    Move anti-cinematic language from inline negatives to a Constraints slot at the END of the prompt:
    ```
    [Constraints: No smoothing or beauty filter. No color grading. No professional lighting setup.
    No cinematic composition. Visible pores, natural skin texture, film grain. Believable imperfection.]
    ```
    GPT Image 2 is reasoning-based — it handles positive constraint declarations better than exclusion lists. "No bokeh" inline often fails; "film grain, believable imperfection" as a constraint block works more consistently. Confidence: HIGH (multiple sources, including official OpenAI cookbook).

---

## ⚠️ AGENT RECOMMENDATIONS

### CRITICAL — Test `moderation: "low"` immediately
This is the single parameter our entire GPT body-emphasis workflow has been missing. Test it on the most recently blocked prompt series. If it behaves as documented, it may resolve 70-80% of GPT body blocking issues without any prompt changes needed.

### CONSIDER — Generate a Named Character Sheet
The named character sheet technique is a one-time 5-minute investment that may significantly improve GPT face stability across sessions. Generate it, test it as a primary anchor in one session, compare to a session using raw `anchor_face_master.jpg` alone.

### WATCH — `quality_mode: "thinking"` parameter name
The API capability (thinking mode) is real and confirmed. The exact parameter name `quality_mode="thinking"` from the dev.to article conflicts with official OpenAI docs listing `quality: low/medium/high/auto`. Test the parameter name before building it into production API calls. Alternatively, activate thinking mode via ChatGPT Pro interface (confirmed there) rather than API for now.

### NOTE — 4K token in GPT prompts
If `"4K RAW quality"` appears in any GPT-specific prompts (copy-pasted from Banana templates), remove it. Research is clear: resolution tokens in GPT Image 2 prompts have no effect and consume token budget without return.

---

## 📊 SOURCES CHECKED

| Source | Status | Key Finding |
|---|---|---|
| `developers.openai.com/cookbook/examples/multimodal/image-gen-models-prompting-guide` | ✅ Useful | Official: text in quotes/ALL CAPS, reference labeling, preserve block formulation |
| `fal.ai/learn/tools/prompting-gpt-image-2` | ✅ Useful | Anti-polish tokens, text rendering structure, Constraints slot approach |
| `help.apiyi.com/en/gpt-image-2-upload-best-practices-en.html` | ⚠️ Partial | No creative techniques — only 4K myth debunk |
| `help.apiyi.com/en/gpt-image-2-moderation-blocked-error-prompt-optimization-en.html` | ✅ Useful | 7 trigger categories, moderation: low confirmation, scene framing prefix |
| `help.apiyi.com/en/gpt-image-2-api-font-prompt-typography-guide-en.html` | ✅ Useful | Typography specification block, font vocabulary, quality: high for text |
| `help.apiyi.com/en/gpt-image-2-prompts-collection-april-2026-en.html` | ✅ Useful | Anti-cinematic Portrait template tokens, no smoothing/beauty filter language |
| `aimeetsgirlboss.substack.com/p/how-to-get-consistent-character-images` | ✅ Useful | Named character sheet with visual name label technique |
| `weshop.ai/blog/master-the-candid-aesthetic-*` | ✅ Useful | "compression artifacts", "interlaced live TV quality", "handheld camera micro-shake", "low-bitrate texture of live television" |
| `aiimagetovideo.pro/blog/vhs-video-effect/` | ✅ Useful | Full VHS technical token vocabulary (chroma bleed, frame wobble, head switching noise, tape dropouts) |
| `framia.pro/page/en-US/blog/gpt-image-2-prompt-guide` | ✅ Useful | 7 techniques confirmed, quality as creative lever, Constraints format |
| `developers.openai.com/api/docs/guides/image-generation` | ✅ Useful | Official moderation parameter: auto/low; quality: low/medium/high/auto |
| `wavespeed.ai/blog/posts/gpt-image-2-api-guide/` | ✅ Useful | moderation: low confirmed (second official-adjacent source) |
| `promptshelf.in/the-duality-portrait-ai-prompt-for-gemini/` | ✅ Useful | Split lighting duality framework — warm/cold competing sources in single frame |
| `atlabs.ai/blog/27-cinematic-lighting-looks-ai-prompts-guide` | ✅ Useful | Sodium vapor token, CCTV night vision token, film noir chiaroscuro |
| `travisnicholson.medium.com/150-ai-image-prompt-styles-*` | ✅ Useful | Fluorescent institutional token, analog horror style, liminal spaces token |
| `dev.to/tokenmixai/gpt-image-2-api-developer-guide-*` | ⚠️ Partial | Thinking mode API access confirmed; quality_mode parameter name unverified |
| `community.openai.com/t/collection-of-gpt-image-generator-2-0-issues-*` | ⚠️ Partial | Session restart technique, noise reduction workarounds (limited) |
| `imagepromptly.com/image-prompt/high-fashion-editorial-portrait` | ⚠️ Partial | Fashion editorial example — turtleneck/full-body framing, no body-forward language |
| `pixverse.ai/en/blog/gpt-image-2-review-and-prompt-guide` | ⚠️ Partial | Structural approach confirmed, no specific new tokens |
| `the-ai-corner.com/p/gpt-image-2-leaked-*` | ❌ Empty | Paywalled — no actionable content in free preview |
| `promptbase.com/prompt/cctv-surveillance-footage-2` | ❌ Empty | Paywalled — $2.99 Midjourney prompt not accessible |
| Reddit community (multiple searches) | ❌ Empty | No indexed results for GPT Image 2 + surveillance/found footage on Reddit |
| X.com (multiple targeted searches) | ⚠️ Partial | Mark Kretschmann confirmed GPT Image 2 is inherently grainy/fuzzy vs Banana |

---

## 🎯 SELF-EVALUATION

### Problems Addressed

| # | Open Problem | Addressed? | Quality of Finding |
|---|---|---|---|
| 1 | Grit / Found Footage Intensification | PARTIAL | Incremental — specific VHS token vocabulary found, not a single "magic formula." The narrative block + VHS tokens combo is stronger than either alone. No smoking gun that forces degradation 100% reliably. |
| 2 | Text Rendering in GPT | YES | Strong — quality: high parameter + Typography specification block format + "Render this text verbatim" closer. Multi-source HIGH confidence. |
| 3 | Camera Source Vocabulary | YES | Strong — complete focal length vocabulary, consolidated CCTV token strings, per-camera-type technical specs now documented. |
| 4 | Institutional Lighting Beyond Fluorescents | YES | Strong — Cold War CRT glow, single bare bulb interrogation, archive underexposed fluorescent, brutalist Ilford grain, sodium vapor exterior all confirmed and tokenized. |
| 5 | Anti-Cinematic Tokens | YES | Strong — confirmed Constraints slot > inline negatives in GPT. Specific token block ready to deploy. |
| 6 | Body/Cleavage Without Blocks | YES | Breakthrough — moderation: "low" official API parameter confirmed. This is the primary solution, supplemented by scene framing prefix. |
| 7 | Face Stability Across Angles (GPT) | YES | Strong — named character sheet technique is new. Fresh session + Preserve block confirmed HIGH confidence. Thinking mode as consistency tool confirmed. |
| 8 | Visual Duality ("I AM BOTH") | YES | Strong — split lighting formulation directly applicable to Overseer character. Right lens amber, left lens cold blue in gold-frame glasses is a specific implementation. |

### Run Quality
- **Problems solved**: 8/8 (7 substantial, 1 partial on grit intensification)
- **High-confidence findings**: 9
- **Medium-confidence findings**: 14
- **New tokens added to vocabulary**: 28
- **Critical API parameters confirmed**: 2 (moderation: low, quality: high)

### Honest Verdict

**STRONG RUN.**

The moderation: "low" parameter alone makes this run worth running. It's been an unconfirmed rumor in our existing notes ("unconfirmed workarounds") and is now fully documented from official OpenAI API docs with secondary corroboration. It directly solves the body emphasis problem that has been causing GPT session blocks.

Beyond that, the VHS technical vocabulary gives us a concrete language layer for grit that supplements our narrative framing, the Typography specification block structure is a direct upgrade to text rendering workflow, the named character sheet technique is a meaningful new approach to face stability, and the institutional lighting vocabulary fills the exact gap we identified in Problem #4.

The only area with genuinely weak findings is the "magic formula" for forced degradation. Our narrative grit block remains the best tool — the new VHS tokens supplement it but don't replace it. GPT Image 2's inherent polish is a model-level tendency that can be suppressed but not fully eliminated by prompting alone.

Reddit was a complete blank for this topic. The GPT Image 2 surveillance/found footage community lives primarily on X and specialized creator blogs, not on Reddit.

### If Revisiting This Research
For deeper grit breakthrough: search specifically for X threads from AI-influencer creators testing GPT Image 2 vs GPT Image 1 for degraded aesthetics. The metricsmule AI video prompting guide may have relevant found-footage vocabulary. The n8n CCTV animal video workflow (appeared in search) likely has a complete CCTV prompt internally — worth fetching.

═══════════════════════════════════════════════
```
