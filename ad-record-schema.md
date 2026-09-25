# Ad Record Schema

Use one row per distinct Library ID. Keep unknown fields blank or `unknown`; never use zero to mean missing.

| Field | Allowed values / notes |
|---|---|
| library_id | String; deduplicate on this field |
| direct_url | `https://www.facebook.com/ads/library/?id=[ID]` |
| advertiser | Visible page/advertiser name |
| country | Source filter, not inferred location |
| active_status | active, inactive, unknown |
| start_date | ISO date when visible |
| format | video, image, carousel, text, unknown |
| platforms | Explicitly displayed platforms only |
| primary_text | Faithful transcription or concise summary |
| headline | Visible headline, otherwise unknown |
| cta | Visible CTA or unknown |
| destination | URL, message, lead form, app, unknown |
| situation | pain, aspiration, event, comparison, education, entertainment, unknown |
| promise | functional, emotional, identity, price, proof-led, unknown |
| proof | testimonial, demo, authority, guarantee, numbers, UGC, none, unknown |
| offer | product, lead magnet, consultation, discount, event, content, unknown |
| journey_hypothesis | cold, education, consideration, conversion, retention, unknown; always a BET |
| evidence_note | Exact observation supporting codes |
| missing_or_ambiguous | What was not visible or may be misread |
