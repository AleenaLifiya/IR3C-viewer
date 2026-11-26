# IR3C viewer: real or reconstructed?

A static page where visitors scroll through MRI volumes and guess whether each was fully
acquired or reconstructed by IR3C from a subset of its slices (uniform mask, one slice in
every 2, 4 or 8 kept). Nothing is logged; guesses stay in the visitor's browser.

* `site/` is the published page (NiiVue 0.44.2 vendored, volumes as 8-bit NIfTI).
* `scripts/make_volumes.py` builds `site/volumes/` and `site/cases.js` from the review exports.

Research images only, not for clinical use. Data: BraTS 2023 adult glioma (validation
release), OAI-ZIB knee MRI (Osteoarthritis Initiative), IXI-tiny (CC BY-SA 3.0).
