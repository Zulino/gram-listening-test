# Audio quality listening test

A blind multi-stimulus listening study: each item is a generated audio clip
rendered by **three different systems**, presented in random order
(Version A / B / C). Raters score the overall audio quality of each version
on a 0–100 scale (Bad / Poor / Fair / Good / Excellent).

**To take part:** open the site and follow the instructions
(headphones recommended, quiet environment). The whole test takes about
10–15 minutes.

Notes for the experimenter:

- Everything runs client-side; there is no backend, no cookies, no tracking.
  Progress is autosaved in the rater's browser only.
- Result submission: automatic if `CONFIG.js` has an Apps Script URL
  (see `apps_script.gs`); otherwise raters copy a one-line result code
  into a Google Form or message. Codes are decoded offline with
  `decode_results.py` (requires `blinding_key.json`, which is **not**
  published — that file holds the letter→system mapping).
- To rebuild the stimuli or the site, see the private experiment folder
  (`listening_test/` in the research repository).

The three systems and the mapping from files to systems are blind to
raters; the analysis and the systems' identities are reported in the paper.
