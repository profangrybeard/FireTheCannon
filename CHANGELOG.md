# Changelog

All notable changes to the *Fire the Cannons!* build guide and project repo.
Newest version on top. See [README.md](README.md) for the live published guide
link.

## v1.2 — 2026-04-26

### Fixed (UE 5.6.1 accuracy)
- **Phase 7** — Projectile Movement property is `Projectile Gravity Scale`,
  not `Project Gravity Scale`. Students searching the Details panel for the
  old wording would find nothing.
- **Phase 11** — Camera Shake parent class is **Matinee Camera Shake** in UE
  5.6 (not "Legacy Camera Shake"). `Location Amplitude` and `Rotation
  Amplitude` aren't flat scalars either — they live nested under
  `Loc Oscillation` (X/Y/Z) and `Rot Oscillation` (Pitch/Yaw/Roll). Step now
  walks through the real property layout.
- **Bonus B** — Pin on `Apply Radial Damage With Falloff` is `Damage Causer`,
  not `Hurt Causer`.

### Changed
- **Phase 6** — Softened the "Wednesday will revisit Get All Actors of Class
  with a better pattern" promise. Wednesday never demoed it, so the gotcha
  now explains the cached-array pattern in place rather than punting.

### Repo
- Added Unreal-flavored `.gitignore` (refreshed Epic template + IDE/OS/crash
  entries).
- Replaced README stub with project overview + asset inventory + link to the
  published GitHub Pages guide.

---

## v1.1 — 2026-04-26

### Added
- Screenshot capture handler in the guide (each 📸 cue now accepts an inline
  image upload, persisted in localStorage).
- Bonus phases B1–B4 (charge shots, ammo inheritance, score HUD, slo-mo).
- Per-section "Resume here" / "Complete section" buttons.
- Dark-mode CSS pass.

### Changed
- Reorganized phases into Monday (1–6) / Wednesday (7–11) / Submission (12)
  with explicit session dividers.

---

## v1.0 — 2026-04-26

### Added
- Initial build guide (Phases 1–12: project setup → Chaos destruction →
  package & submit).
- Naming-convention table (`BP_`, `IA_`, `IMC_`, `SM_`, `M_`, `NS_`, `S_`,
  `MAP_`, `GC_`).
- Submission rubric and self-check.
- GitHub Actions workflow to deploy the guide to GitHub Pages on push to
  `main`.

---

## Versioning

- **Patch** (v1.x → v1.x+1): typos, pin / property name corrections, broken
  link fixes. No behavioral change to what students build.
- **Major** (v1.x → v2.0): new phase, restructured section, new bonus, or
  any change that affects what the rubric checks.
- **No bump**: same-day touch-ups while iterating before students start the
  assignment.
