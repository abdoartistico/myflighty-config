# myflighty-config

Remote config for the MyFlighty Android app (`com.flighty.yourflighty`). The app fetches
`config.json` on every launch — edit it here and every installed copy picks it up, no update needed.

- `adsb_lol_base`, `adsb_fi_base` — optional ADS-B API overrides (empty = the public endpoints)
- `ad_network` — `admob` | `meta` | `pangle` | `levelplay` | `none` (no ads at all)
- `ad_ids`, `features`, `settings` — ad units, which ad spaces are on, frequency
  (`interstitial_every_n`, `interstitial_cooldown_seconds`, `rewarded_ad_free_minutes`)
- `review` — the "Rate MyFlighty" prompt (after `min_opens_before_prompt` app launches, then at most every `days_between_prompts` days)
- `maintenance`, `update`, `telegram` — gates and promo, off unless `enabled: true`
