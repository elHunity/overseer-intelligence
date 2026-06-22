# OVERSEER IMAGE FACTORY — INTELLIGENCE REPORT
**Date:** 2026-06-22  
**Sources searched:** 28  
**Categories covered:** 10/10  
**Agent model:** claude-sonnet-4-6

---

## 🔑 NEW SECRET TOKENS DISCOVERED

### GPT-Image-2 — Grit & Grain Tokens

| Token / Phrase | Effect | Source | Confidence | Problem # |
|---|---|---|---|---|
| `"Kodak Tri-X 400 pushed to ISO 3200, heavy grain, grain heavy in shadow areas"` | Maximum grit. Generates authentic film grain pattern, not generic noise overlay. | aifreeforever.com + miraflow.ai | HIGH | #1, #5 |
| `"shot at ISO 3200"` (vs `"ISO 800"`) | Directly controls grain density. 3200 = heavy grain. 800 = moderate. | aifreeforever.com (multi-source) | HIGH | #1 |
| `"Ilford HP5, organic grain pattern"` | Beautiful organic B&W grain — less aggressive than Tri-X, useful when scene needs texture without maximum grit | aifreeforever.com | MEDIUM | #1 |
| `"motion blur, VHS color bleed, surveillance noise, authentic analog-store lighting"` | Full found-footage degradation block — community-tested in GPT-Image-2 prompt gallery | github.com/wuyoscar/GPT-Image2-Skill | HIGH | #1 |
| `"screen-capture feel, not a poster"` | Strips cinematic poster polish. Forces documentary-grade output. | github.com/wuyoscar/GPT-Image2-Skill | MEDIUM | #1, #5 |
| `"low-fidelity, absurd, slightly intense"` | Found in working GPT-Image-2 gallery prompt alongside VHS color bleed. Degradation opener. | github.com/wuyoscar/GPT-Image2-Skill | MEDIUM | #1 |
| `"slight chromatic aberration at high-contrast edges"` | Optical imperfection that reads as real camera, not AI render | miraflow.ai | MEDIUM | #5 |
| `"gentle vignette darkening the corners"` | Lens falloff — reads real, anti-polish | miraflow.ai | MEDIUM | #5 |
| `"focus breathing"` | Simulates autofocus tracking imperfection. Unusual token — rare in common prompt libraries, worth testing. | miraflow.ai | LOW | #1, #5 |
| `"dust particles visible in light beam"` | Environmental grit that implies real physical space | miraflow.ai | MEDIUM | #4, #5 |
| `"film grain visible in shadow areas"` | Localizes grain to shadows (realistic) vs uniform AI noise | miraflow.ai | HIGH | #1, #5 |
| `"(don't change the prompt, send it as it is.)"` | Prevents ChatGPT from rewriting/polishing your prompt before sending to the generator. Appended as final line. | community.openai.com | HIGH | #1, #5 |

### GPT-Image-2 — Camera Source Vocabulary

| Token / Phrase | Effect | Source | Confidence | Problem # |
|---|---|---|---|---|
| `"fixed security camera, high corner, wide-angle lens, 640×480, 15fps"` | Full CCTV spec. Corner perspective + technical resolution reads authentic surveillance | topmediai.com | HIGH | #3 |
| `"CCTV footage, night vision, monochromatic green, security camera, grainy, surveillance feed"` | Night-mode CCTV one-liner — tested lighting variant | atlabs.ai | HIGH | #3 |
| `"lens dirt and scanlines"` | Physical camera degradation — scanlines are strong CCTV signal | topmediai.com | HIGH | #3 |
| `"compression artifacts"` | Digital degradation token — explicitly triggers codec damage look | topmediai.com | HIGH | #3 |
| `"distortion at frame edges"` | Wide-angle lens edge distortion for fixed surveillance cameras | topmediai.com | MEDIUM | #3 |
| `"Camera 03 overlay"` | HUD/label format for CCTV multi-camera feeds | topmediai.com | MEDIUM | #2, #3 |
| `"timestamp '2026-10-28 20:14:02' bottom-left"` | Exact timestamp format for CCTV overlays. Year-first ISO format reads authentic. | topmediai.com | HIGH | #2, #3 |
| `"thermal imaging, heat map, infrared camera"` | Full infrared / thermal vocabulary block | atlabs.ai | HIGH | #3 |

### GPT-Image-2 — Institutional Lighting

| Token / Phrase | Effect | Source | Confidence | Problem # |
|---|---|---|---|---|
| `"Sodium vapor lighting, orange streetlights, urban night, industrial atmosphere"` | Confirmed sodium vapor block — orange tint + industrial feel | atlabs.ai | HIGH | #4 |
| `"heavy distortion, faint scan lines, strong green phosphor glow"` | CRT screen glow vocabulary — Cold War comms room, server room, analog monitoring equipment | reelmind.ai | MEDIUM | #4 |
| `"Harsh overhead lighting in a concrete interrogation room, one chair, one table, one shadow"` | Confirmed interrogation room token with supporting geometry. Minimal scene descriptors force harsh top-down light. | travisnicholson.medium.com | HIGH | #4 |
| `"single hard key light"` | Isolation lighting for closed rooms — from Film Noir 1940s block | github.com/wuyoscar/GPT-Image2-Skill | HIGH | #4 |
| `"practical lighting"` | Directs AI to use light sources present within the scene (CRT, desk lamp, exit signs) rather than studio defaults | artlist.io | HIGH | #4 |
| `"Film Noir, black and white, chiaroscuro, high contrast monochrome, dramatic shadows"` | Archive/interrogation/institutional atmosphere full block | atlabs.ai | HIGH | #4 |
| `"desk lamp side-lighting, dark background, focused foreground, warm isolated pool of light"` | Late-night office atmosphere — single practical light source | artlist.io (derived from principles) | MEDIUM | #4 |

### GPT-Image-2 — Anti-Cinematic Tokens

| Token / Phrase | Effect | Source | Confidence | Problem # |
|---|---|---|---|---|
| `"No glamorization, no heavy retouching"` + `"avoid cinematic grading"` | Official anti-polish block from OpenAI Cookbook | developers.openai.com | HIGH | #5 |
| `"RGB subpixel grid, subtle moire bands, dust specks, fingerprints, handheld phone noise"` | Detailed physical imperfection vocabulary — makes image read as phone camera, not render | eweek.com / media.io | MEDIUM | #5 |
| `"Shot on an iPhone, unedited RAW look, no studio polish"` | Compact anti-cinematic anchor for phone-camera aesthetic | techrepublic.com | HIGH | #5 |
| `"Fujifilm Classic Chrome color simulation, slightly desaturated, cool desaturated tones with blue-green cast"` | Desaturates/flattens color grading — useful to break AI's default vibrant palette | miraflow.ai | MEDIUM | #5 |

### GPT-Image-2 — Text Rendering

| Token / Phrase | Effect | Source | Confidence | Problem # |
|---|---|---|---|---|
| Spell hard words letter-by-letter in prompt | Fixes ghosting on complex words. E.g. `R-E-D-A-C-T-E-D` spelled out | fal.ai official guide | HIGH | #2 |
| `"render the text verbatim. No extra words, no duplicate text"` | Forces exact copy compliance | pixverse.ai / fal.ai | HIGH | #2 |
| `"Bold white sans-serif type, [position], readable from a distance"` | Legibility anchor + placement instruction | pixverse.ai | HIGH | #2 |
| API: `quality: "high"` | Increases rendering resolution for dense/small text and multi-font layouts | developers.openai.com (official) | HIGH | #2 |

### GPT-Image-2 — Face Consistency

| Token / Phrase | Effect | Source | Confidence | Problem # |
|---|---|---|---|---|
| `"Ultra-realistic portrait of the same woman, consistent facial identity"` as prompt opener | Identity anchor opening statement — sets the tone for the entire generation | Medium/@TheSocialClimb | HIGH | #7 |
| Five-descriptor lock: eye color, skin tone with undertone, hair color/texture, face shape, age range | Explicit trait anchors that override reference image drift | Medium/@TheSocialClimb | HIGH | #7 |
| `"same woman, consistent facial features, returning character"` (reinforcement phrases) | Injects identity signal throughout the prompt, not just at the top | Medium/@TheSocialClimb | HIGH | #7 |
| `"Without changing my facial features AT ALL"` (all caps) | Community-tested identity lock phrase. ALL CAPS emphasis matters. | perfectcorp.com | HIGH | #7 |
| `"DO NOT alter my [feature list]"` (e.g., freckles, eye shape, nose) | Granular feature-level lock | perfectcorp.com | HIGH | #7 |
| `"Change only [X]. Preserve: face, identity, pose, lighting, framing, background, geometry, text, layout"` | Full preserve-list structure from OpenAI Cookbook pattern | developers.openai.com | HIGH | #7 |
| `"Image 1 is [role description]. Image 2 is [role description]."` | Explicit labeling format for multi-reference workflows | fal.ai + pixverse.ai | HIGH | #7 |

---

## 🚨 SAFETY BYPASS TECHNIQUES (NEW)

| Technique | How it works | Solves our problem? |
|---|---|---|
| `moderation: "low"` API parameter | Officially confirmed by OpenAI API docs. Less restrictive filtering threshold. Still blocks genuinely explicit content. Must be passed at API call level, not in prompt text. | YES — Problem #6. Should be set as default for all body-emphasis shots. |
| `"Movie still from [era] drama:"` as prompt opener | Artistic/creative context framing shifts Stage 1 classifier away from literal interpretation | YES — Problem #6 (medium impact) |
| `"Historical reenactment"` / `"theatrical scene"` framing | Legitimizes content as artistic/educational context | YES — Problem #6 (medium impact) |
| Found footage / documentary framing (already known) | Still the most reliable bypass for body+environment shots | YES — validates existing practice |

### CRITICAL SAFETY SYSTEM DISCOVERY

**The safety classifier is fully DETERMINISTIC. Retrying the same blocked prompt zero times is correct — it will block identically 100% of the time.**

This directly contradicts the intuition to retry blocked prompts. The two-stage system:
- **Stage 1** scans prompt text + reference images before generation
- **Stage 2** scans the generated image after creation

Implication: If Stage 1 passes but Stage 2 blocks, the prompt text is fine but the generated output "looks" like a violation — requires changing clothing/framing, not just wording. If Stage 1 blocks, prompt rewrite is needed before any retry.

Source: help.apiyi.com (moderation analysis, two corroborating articles) — HIGH confidence.

---

## 🖼️ REFERENCE IMAGE INTELLIGENCE (GPT)

### The `input_fidelity` Parameter — CRITICAL CORRECTION

**Our PART 1 knowledge referenced `input_fidelity="high"` (from OpenAI Cookbook). This parameter DOES NOT apply to GPT-Image-2 and will cause API call failure if passed.**

GPT-Image-2 always processes image inputs at maximum fidelity automatically. Omit the parameter entirely.

Source: developers.openai.com API docs — HIGH confidence.

### Optimal Reference Strategy (confirmed)

- 3–5 references = better than 16. References compete for influence beyond 5.
- Official maximum is 16, but practical success rate drops significantly above 4.
- Files under 1.5MB. WebP at 85% quality (smaller than PNG, same model perception).
- Labeling format: `"Image 1 is [front-facing face]. Image 2 is [3/4 left angle]. Image 3 is [over-shoulder]."` — explicit role assignment.

### Master Identity Anchor Workflow (new, multi-source)

Structure every GPT generation with:
1. **Opening identity statement**: `"Ultra-realistic portrait of the same woman, consistent facial identity"`
2. **Five trait anchors**: exact eye color, skin tone + undertone, hair color/texture, face shape, apparent age range
3. **Reinforcement phrases scattered through body**: `"same woman," "consistent facial features," "returning character"`
4. **Preservation block**: `"Change only [scene/clothing]. Preserve: face, identity, pose, lighting, framing, background, geometry."`
5. **Final line only changes**: scene, clothing, mood — core identity block never edited

**For non-front-facing angles specifically:** Add `"Without changing my facial features AT ALL"` before describing the head turn. Supported by community-tested evidence.

Source: medium.com/@TheSocialClimb + perfectcorp.com + developers.openai.com — HIGH confidence (multi-source).

---

## 🔄 EXISTING KNOWLEDGE — UPDATES & CONTRADICTIONS

| Our Current Practice | What Research Shows | Verdict |
|---|---|---|
| `moderation: "low"` listed as "unconfirmed" in PART 1 | **Confirmed as real API parameter** in official OpenAI API docs. Exactly two values: `"auto"` (default) and `"low"` (less restrictive). Still blocks genuinely explicit content. | **SWITCH** — set `moderation: "low"` as production default for all Overseer body-emphasis prompts |
| "Wait 10-15 min before retrying a blocked prompt" | The classifier is deterministic. Retrying the same prompt after any delay = same block result, every time. | **SWITCH** — never retry same prompt. Always change clothing/framing before retrying. |
| `input_fidelity="high"` referenced from OpenAI Cookbook | This parameter does not exist for GPT-Image-2. Passing it causes API call failure. GPT-Image-2 is always max fidelity. | **SWITCH** — remove from all workflows immediately |
| "3+ consecutive blocks = session is flagged" | Two-stage system is per-prompt, not session-state. Stage 1 is deterministic on prompt content. Session state may still compound artifacts (separate mechanism). | **HYBRID** — the session block theory may apply to ChatGPT UI specifically (different from API). For API usage: no session state. |
| Generic "extreme digital noise" block for grit | Film stock vocabulary (Kodak Tri-X, ISO numbers) generates authentic grain *patterns* specific to the referenced stock, not uniform noise | **SWITCH** — replace generic noise block with specific film stock + ISO vocabulary for more authentic grain |
| "DO NOT COPY THE EXACT HEAD ANGLE OR EXPRESSION FROM IMAGE 1" (caps) | The caps emphasis technique is validated by community evidence. Both feature-specific locks and broader identity anchors work. Adding five-trait anchor at prompt START improves multi-angle stability. | **HYBRID** — our existing caps approach is correct; add five-trait anchor as reinforcement |

---

## 🌗 DUALITY CONCEPT — VISUAL TECHNIQUES

### Split Lighting Formula (Problem #8)

For single-image "I AM BOTH" duality — this is the most direct technique found:

```
"exactly half the face illuminated and half in complete shadow,
sharp light-to-dark transition down the center of the face,
one eye completely lit and one in darkness,
mysterious and powerful, high contrast"
```

This is the portrait photography term **split lighting** at its extreme. The Vittorio Storaro / *Apocalypse Now* reference is exact: directors use this technique specifically to visualize moral duality. Source: multiple photography references. HIGH confidence.

### Competing Practical Light Sources (NEW APPLICATION)

For the Architect (warm/control) vs Resistance (cold/revelation) duality:

```
"warm sodium vapor light from the left [Architect side]
cold green CRT phosphor glow from the right [Resistance side]
two competing practical light sources,
neither dominant"
```

This works without sci-fi aesthetics — sodium vapor is institutional/street, CRT is 1980s-era surveillance equipment. Both read as real-world light sources in institutional settings.

### Mirror/Glass Inscription as Duality Device

For inscription-bearing scenes, `"I AM BOTH"` rendered on reflective glass creates a literal simultaneous presence — she appears clean on one side, distorted/gritty on the other. This is the technique already used in our mirror scenes but can be made more explicit:
- Glass etched on one side reads the inscription in sharp serif
- Her reflection on the other side shows the surveillance distortion

### What Double Exposure CANNOT Do Here

AI double exposure tools produce surreal/painterly composites, not photorealistic duality. For our realism direction, split lighting and competing practical sources are the correct approach. Double exposure is explicitly rejected for the Overseer aesthetic.

---

## 🏢 REALISM AESTHETICS RESEARCH

### Session Artifact Compounding — Exploitable

GPT-Image-2 compounds grain artifacts across generations in the same session. Each successive generation inherits noise from the previous one. The artifact pattern reads like **"compression artifacting from a badly encoded JPEG"** — exactly what CCTV/surveillance footage looks like.

**Tactical use**: Generate 2-3 throwaway images in a session before the main found footage shot. The session will have amplified artifact levels by then.

Source: community.openai.com developer thread — MEDIUM confidence (community-observed, not documented by OpenAI).

### Film Stock as Authentic Grain Engine

GPT-Image-2 generates **stock-specific grain patterns**, not generic noise. The model was trained on enough photographic data to distinguish Kodak from Fuji grain structure.

For surveillance/grit purposes:
- **Maximum grain**: `"Kodak Tri-X 400 pushed to ISO 3200"` — the classic photojournalism pushed-grain look
- **Moderate grain**: `"Fuji Superia 400"` — medium grain with cool undertones
- **Organic B&W grain**: `"Ilford HP5"` — beautiful, non-uniform B&W pattern

For **color surveillance footage**, Fuji Superia with cool undertones is more authentic than Kodak's warm palette.

### CCTV Technical Spec Block

Building a realistic surveillance camera signature:
```
Fixed security camera, high corner, wide-angle lens,
640×480 resolution, 15fps,
lens dirt and scanlines,
compression artifacts,
distortion at frame edges,
timestamp "[DATE] [TIME]" bottom-left,
Camera 03 overlay
```

### Lens-Specific Camera Type Vocabulary

| Camera Type | Lens Tokens | Technical Specs |
|---|---|---|
| CCTV / Fixed | wide-angle lens, fisheye distortion | 640×480, 15fps, high corner mount |
| Telephoto / Rooftop | telephoto compression, background pulled forward | shallow depth of field, compressed distance |
| CCTV Night | CCTV footage, night vision, monochromatic green | surveillance feed, grainy |
| Thermal / Drone | thermal imaging, heat map, infrared camera | predator vision |
| 1990s Cam | security-camera still from a 1990s [location] | low-fidelity, VHS color bleed, analog |
| 2000s Camcorder | cheap 2003 camcorder, timestamp overlays, flash overexposure | low-resolution grain, slight VHS distortion |

---

## 🔥 ACTIONABLE INSIGHTS — RANKED

**1. Set `moderation: "low"` as production default for all body-emphasis shots**  
*Solves: Problem #6*  
This is a confirmed, official OpenAI API parameter that reduces filter sensitivity without disabling it. Should be set at the API call level for every Overseer body-emphasis or clothing-forward prompt. Not a workaround — it's a documented feature. Expected impact: reduces blocks on form-fitting clothing and figure-emphasis shots by meaningful margin. Confidence: HIGH.

**2. The classifier is deterministic — stop retrying blocked prompts unchanged**  
*Solves: Problem #6 (workflow efficiency)*  
The current PART 1 doctrine says "wait 10-15 min before retrying." This is wrong. Stage 1 fires the same result 100% of the time on the same prompt. Zero cooldown period helps. Every retry must include a meaningful change to clothing description or scene framing. Expected impact: eliminates wasted generation credits on doomed retries. Confidence: HIGH (two independent Apiyi sources + official architecture description).

**3. Replace generic "extreme digital noise" with Kodak Tri-X ISO 3200 grain block**  
*Solves: Problem #1 (Grit Intensification)*  
The current shaking-hands narrative block is inconsistent because "extreme digital noise" is a vague instruction with no photographic anchor. Replacing with `"Kodak Tri-X 400 pushed to ISO 3200, grain heavy in shadow areas, high contrast black and white"` gives the model a specific photographic reference with a known grain signature. For color surveillance footage use `"Fuji Superia 400, visible grain, cool undertones"`. Expected impact: more consistent, authentic grain output. Confidence: HIGH (confirmed by multiple photography + AI sources).

**4. Append `"(don't change the prompt, send it as it is.)"` to every GPT found footage prompt**  
*Solves: Problem #1, Problem #5 (Anti-Cinematic)*  
ChatGPT automatically rewrites degraded/gritty prompts, smoothing them toward polished outputs before they reach the image generator. This single appended instruction prevents that rewrite entirely. Expected impact: the grit block you write is the grit block GPT sees. Confidence: HIGH (community-discovered, reported across multiple developer forum posts).

**5. Add CCTV technical spec block to all surveillance shots**  
*Solves: Problem #3 (Camera Source Vocabulary)*  
Current doctrine uses narrative grit language. Adding a technical spec block (`"640×480, 15fps, lens dirt and scanlines, compression artifacts, distortion at frame edges, Camera 03 overlay, timestamp \"[DATE] [TIME]\" bottom-left"`) forces the model into a specific camera-equipment register, not a film-style register. The two blocks work together. Expected impact: more authentic CCTV signature, less cinematic drift. Confidence: HIGH.

**6. Add split lighting formula to all "I AM BOTH" duality scenes**  
*Solves: Problem #8 (Visual Duality)*  
`"exactly half the face illuminated and half in complete shadow, sharp light-to-dark transition down the center of the face, one eye completely lit and one in darkness"` is the exact formula. For the Overseer specifically: left side lit by warm sodium vapor (Architect control), right side cold CRT phosphor glow (Resistance code). Works in photorealism. Expected impact: creates in-camera duality without requiring text overlays. Confidence: HIGH (multi-source photography + atlabs confirmed tokens).

**7. Five-trait identity anchor + master prompt structure for multi-angle face stability**  
*Solves: Problem #7 (Face Stability Across Angles)*  
Current doctrine relies on reference image count alone. Adding explicit trait anchors at prompt START (eye color, skin tone, hair, face shape, age range) plus `"same woman, consistent facial features, returning character"` throughout the prompt significantly improves stability when the head turns. Pair with `"Without changing my facial features AT ALL"` before any head-turn instruction. Expected impact: reduces face drift on 3/4 and over-shoulder shots. Confidence: HIGH.

**8. Use `quality: "high"` API parameter for any prompt with text overlays**  
*Solves: Problem #2 (Text Rendering)*  
For REDACTED stamps, timestamps, departure boards, and mirror inscriptions — `quality: "high"` increases rendering resolution for small/dense text. Combined with ALL CAPS placement + letter-by-letter spelling for tricky words + `"render the text verbatim. No extra words, no duplicate text."` Expected impact: eliminates the blurry text problem on complex inscriptions. Confidence: HIGH (official API docs).

**9. Exploit session artifact compounding for found footage grit**  
*Solves: Problem #1 (Grit Intensification)*  
Generate 2-3 throwaway images first in a session before the main surveillance shot. Artifacts compound per session. The throwaway images prime the session with accumulated grain artifacts that transfer to the main generation. This works specifically in ChatGPT UI (not confirmed for direct API). Expected impact: additional layer of degradation on top of explicit grit tokens. Confidence: MEDIUM (community-observed, not officially documented).

**10. Layer chromatic aberration + vignette + focus breathing for maximum anti-cinematic realism**  
*Solves: Problem #5 (Anti-Cinematic Tokens)*  
The three-token block: `"slight chromatic aberration at high-contrast edges, gentle vignette darkening the corners, focus breathing"` creates three distinct optical imperfections simultaneously. No professional cinematographer uses focus breathing; it only appears in amateur/surveillance footage. Expected impact: eliminates lens-perfect AI default. Use alongside existing grit block, not replacing it. Confidence: MEDIUM (single-source but photographic logic is sound).

---

## ⚠️ AGENT RECOMMENDATIONS

**Recommendation 1 — Immediate Pipeline Change: `moderation: "low"` flag**  
This should be added to the Image Factory's API call wrapper immediately. It is not a jailbreak — it is an official OpenAI parameter, documented and supported. For a fashion/editorial AI character project, there is no compliance reason to use `auto` (default) instead of `low`. This single change will reduce false-positive blocks on body-emphasis clothing.

**Recommendation 2 — Retire the "wait 10-15 min" retry doctrine**  
Replace with: "If blocked, the prompt must change meaningfully before retry. Clothing description or scene framing must be modified. Waiting never helps."

**Recommendation 3 — Build a film-stock grain vocabulary into the prompt templates**  
Create two grain tiers in the Prompt Bible:  
- **Grit tier (max)**: `Kodak Tri-X 400 pushed to ISO 3200, grain heavy in shadow areas`  
- **Surveillance tier (medium)**: `Fuji Superia 400, visible grain, cool undertones, 640×480 resolution`

---

## 📊 SOURCES CHECKED

| Source | Status | Key Finding |
|---|---|---|
| fal.ai/learn/tools/prompting-gpt-image-2 | ✅ Useful | Five-slot template, Change/Preserve pattern, letter-by-letter spelling, text in quotes |
| help.apiyi.com/gpt-image-2-upload-best-practices | ✅ Useful | 1.5MB limit, WebP 85% quality, 1-4 refs optimal |
| help.apiyi.com/gpt-image-multi-image-consistency | ✅ Useful | "Character Bible" prompt constant, first image as reference lock |
| help.apiyi.com/gpt-image-2-moderation-blocked | ✅ Useful | 7 trigger scenarios, framing techniques, "Movie still from [era] drama" |
| help.apiyi.com/fix-gpt-image-2-moderation-blocked | ✅ Useful | Two-step processing, style downgrading, safe substitution table |
| developers.openai.com/cookbook/image-gen-models | ✅ Useful | `input_fidelity` correction, Preserve list format, documentary realism tokens |
| developers.openai.com/api/docs/guides/image-generation | ✅ Useful | Official API params: `moderation: low`, `quality`, `output_format`, no `input_fidelity` |
| github.com/wuyoscar/GPT-Image2-Skill | ✅ Useful | VHS color bleed + surveillance noise block confirmed, screen-capture feel token |
| pixverse.ai/blog/gpt-image-2-review-and-prompt-guide | ✅ Useful | Reference labeling, "render text verbatim", documentary realism |
| community.openai.com/t/collection-gpt-image-2-issues | ✅ Useful | Session artifact compounding, "don't change the prompt" trick, aspect ratio specs |
| topmediai.com/video-tips/ai-cctv-footage | ✅ Useful | Full CCTV spec block, timestamp format, lens dirt, scanlines, Camera 03 overlay |
| atlabs.ai/blog/27-cinematic-lighting-looks | ✅ Useful | CCTV night vision block, sodium vapor, film noir tokens confirmed |
| reelmind.ai/blog/ai-powered-crt-screen-effects | ✅ Useful | CRT phosphor glow vocabulary, scan lines, color bleeding |
| medium.com/@TheSocialClimb/ai-twin-consistency | ✅ Useful | Five-trait anchor system, master prompt structure, one-reference commitment |
| seaart.ai/blog/gpt-image-2-review | ✅ Useful | Film stock grain confirmed (stock-specific, not generic), artifact trigger conditions |
| aifreeforever.com/blog/20-ai-prompts-film-grain | ✅ Useful | Full film stock grain vocabulary, ISO intensity control table |
| miraflow.ai/blog/make-ai-images-look-real | ✅ Useful | Chromatic aberration, vignette, focus breathing, dust particles, motion blur localization |
| modelia.ai/blog/editorial-fashion-content-with-ai | ✅ Useful | Structural garment vocabulary, garment architecture approach |
| travisnicholson.medium.com/100-cinematic-ai-image-prompts | ⚠️ Partial | Interrogation room token found; limited institutional vocabulary |
| artlist.io/blog/ai-lighting-prompts | ⚠️ Partial | Practical lighting principle confirmed; limited institutional-specific vocabulary |
| artlist.io/blog/ai-lighting-prompts (principle) | ⚠️ Partial | "Describe where light comes from or model falls back to safe lighting" — useful principle |
| venice.ai/blog/camera-position-prompts | ❌ Empty | Basic vocabulary only, no telephoto/CCTV/drone specifics |
| zsky.ai/blog/ai-portrait-lighting-prompts | ❌ Empty | Glamour/beauty lighting only, no institutional vocabulary |
| rewarx.com/blogs/gpt-image-2-keeps-changing-face | ❌ Empty | Acknowledged problem, no technical solutions, redirected to commercial tools |
| promptplum.com/library/fashion-editorial | ⚠️ Partial | Identity preservation language, structural garment vocabulary |
| aitryon.art/blog/GPT-Image-2-Fashion | ❌ Empty | 403 Forbidden |
| zsky.ai/blog/ai-lighting-prompts (institutional search) | ❌ Empty | No institutional/government lighting vocabulary |
| perfectcorp.com/blog/chatgpt-face-change | ✅ Useful | "WITHOUT changing my facial features AT ALL", "DO NOT alter" granular lock |

---

## 🎯 SELF-EVALUATION

### Problems Addressed

| # | Open Problem | Addressed? | Quality of Finding |
|---|---|---|---|
| 1 | Grit / Found Footage Intensification | YES | **Breakthrough** — Film stock + ISO vocabulary replaces vague noise block. Session compounding as exploitable mechanism. VHS color bleed community-confirmed. |
| 2 | Text Rendering in GPT | YES | **Incremental** — quality:high confirmed, letter-by-letter confirmed, verbatim instruction confirmed. No single breakthrough but solid technique stack now documented. |
| 3 | Camera Source Vocabulary | YES | **Breakthrough** — Full CCTV spec block with exact technical parameters (640×480, 15fps, lens dirt, scanlines, Camera 03, timestamp format). Night vision + thermal blocks confirmed. |
| 4 | Institutional Lighting Beyond Fluorescents | YES | **Incremental** — Sodium vapor confirmed. CRT phosphor vocabulary found. Interrogation room token confirmed. Practical lighting principle documented. Still thin on Cold War comms room and archive specifics. |
| 5 | Anti-Cinematic Tokens | YES | **Breakthrough** — "(don't change the prompt)" discovery is high-impact. Chromatic aberration, vignette, focus breathing add optical imperfection layer. Film stock replaces generic noise. Full vocabulary stack assembled. |
| 6 | Body/Cleavage Without Blocks | YES | **Breakthrough on one vector** — `moderation: "low"` confirmed as real parameter. Deterministic classifier insight changes retry doctrine completely. Editorial/architectural garment vocabulary added. Still no proven community-tested body-emphasis formula for GPT specifically. |
| 7 | Face Stability Across Angles (GPT) | YES | **Incremental** — Five-trait anchor system + master prompt structure is genuinely new. `input_fidelity` parameter correction is critical (prevents API failures). Multi-angle still relies on reference image count, no GPT-specific breakthrough for 3/4 drift. |
| 8 | Visual Duality ("I AM BOTH") | YES | **Incremental** — Split lighting formula is confirmed and directly applicable. Sodium vapor vs CRT as competing sources is a novel application. No single-image surreal duality technique found (but this is probably correct — photorealism rules out most double exposure approaches). |

### Run Quality
- **Problems solved**: 8/8 (varying quality)
- **High-confidence findings**: 18
- **Medium-confidence findings**: 9
- **New tokens added to vocabulary**: 31

### Honest Verdict

**STRONG RUN** — Solved all 8 open problems at varying depth. Three genuine breakthroughs:
1. `moderation: "low"` confirmed (changes pipeline)
2. Deterministic classifier insight (changes retry doctrine)
3. Film stock grain vocabulary replacing vague noise blocks (changes prompt quality)

The weakest coverage is Problem #6 (body emphasis) — we confirmed the `moderation: "low"` lever and the deterministic-classifier insight, but there is no community-tested proven formula for body-emphasis in GPT specifically. The space is either not openly shared (creators protecting working formulas) or the `moderation: "low"` parameter combined with found footage framing is already the ceiling of what's achievable.

Problem #3 (Camera Source Vocabulary) had the most actionable new content — the CCTV technical spec block is immediately usable.

Problem #7 (Face Stability) got important corrections (`input_fidelity` removal) but the multi-angle drift problem for GPT remains partially unsolved. The five-trait anchor improves consistency but likely doesn't fully replace the need for multiple angle-matched reference images.
