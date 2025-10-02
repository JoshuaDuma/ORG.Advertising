# Duma Realty Branding Repository

This repository is the **single source of truth** for Duma Realty Inc. branding assets, design files, and print-ready exports. It is structured to support professional version control of design work (business cards, signage, logos, and more) using Git + Git LFS.

---

## 📂 Repository Structure

```
dumarealty-branding/
├─ branding/             # Core brand assets
│  ├─ color/             # Palettes (JSON + swatches)
│  ├─ typography/        # Specimens & font licenses
│  └─ logo/              # Logos (src, svg, exports)
├─ business-card/        # Business card designs
│  ├─ src/               # Working files (.ai, .psd, .indd) – LFS
│  ├─ exports/           # Print-ready & web exports
│  ├─ proofs/            # Low-res proofs for review
│  └─ notes.md           # Print specifications & vendor details
├─ signage/              # For sale / sold signs & print materials
│  ├─ src/               # Working files – LFS
│  └─ exports/           # Final exports
├─ web/                  # Brand tokens & web-optimized assets
│  ├─ tokens/            # JSON/SCSS variables (colors, spacing)
│  └─ public/brand/      # Optimized SVG/PNG for website
└─ ops/                  # Operational notes & scripts
   ├─ print-runs.csv     # Log of all print runs
   └─ scripts/           # Helper scripts (renaming, exporting)
```

---

## ⚙️ Git & Git LFS Setup

This repo uses **Git Large File Storage (LFS)** for heavy binary assets.

### Install Git LFS

```bash
brew install git-lfs   # macOS
# or use your OS package manager

git lfs install
```

### Track Design Files

```bash
git lfs track "*.psd" "*.ai" "*.indd" "*.pdf" "*.png" "*.jpg"
git add .gitattributes
git commit -m "chore: track design binaries with LFS"
```

---

## 📝 Workflow

1. **Branch per concept** – e.g., `concept/navy`, `concept/mono`
2. **Work in `/src/`** – commit `.ai`/`.psd` working files
3. **Export to `/exports/`** – commit print-ready PDFs and PNGs
4. **Proofs in `/proofs/`** – low-res versions for quick review
5. **Tag approved runs** – e.g., `v1.0-card-2025-10-01`
6. **Log in `/ops/print-runs.csv`** – track vendor, stock, qty, file

---

## 🖨️ Print Notes

Each project (e.g., business cards, signage) has a `notes.md` file with:

* Vendor & order link
* Size, bleed, safe area
* Color profile (CMYK/ICC)
* Paper stock & finish
* Date, quantity, approval
* File used for print

---

## 🏷️ Naming Conventions

* **Working files (src):** `duma-card_A_v03.ai`
* **Exports:** `duma-card_v1.0_print.pdf` / `duma-card_v1.0_web.png`
* **Branches:** `concept/navy`, `tweak/qr-spacing`
* **Tags:** `v1.0-card-2025-10-01`

---

## 🚀 Usage

Clone and set up LFS before working:

```bash
git clone <repo-url>
cd dumarealty-branding
git lfs install
```

When starting a new design:

```bash
git checkout -b concept/new-idea
```

When finalizing a print run:

```bash
git tag -a v1.0-card-2025-10-01 -m "First print run"
git push --tags
```

---

## 📌 Notes

* **Fonts:** Only include licenses/specimens if redistribution is restricted.
* **SVG preferred:** Use vector exports for web where possible.
* **Binary bloat:** Archive legacy print zips outside the repo if storage/bandwidth becomes an issue.

---

## 📄 License

Internal use only – Duma Realty Inc. branding materials. Not for public redistribution.

# Duma Realty Branding Repository

This repository is the **single source of truth** for Duma Realty Inc. branding assets, design files, and print-ready exports. It is structured to support professional version control of design work (business cards, signage, logos, and more) using Git + Git LFS.

---

## 📂 Repository Structure

```
dumarealty-branding/
├─ branding/             # Core brand assets
│  ├─ color/             # Palettes (JSON + swatches)
│  ├─ typography/        # Specimens & font licenses
│  └─ logo/              # Logos (src, svg, exports)
├─ business-card/        # Business card designs
│  ├─ src/               # Working files (.ai, .psd, .indd) – LFS
│  ├─ exports/           # Print-ready & web exports
│  ├─ proofs/            # Low-res proofs for review
│  └─ notes.md           # Print specifications & vendor details
├─ signage/              # For sale / sold signs & print materials
│  ├─ src/               # Working files – LFS
│  └─ exports/           # Final exports
├─ web/                  # Brand tokens & web-optimized assets
│  ├─ tokens/            # JSON/SCSS variables (colors, spacing)
│  └─ public/brand/      # Optimized SVG/PNG for website
└─ ops/                  # Operational notes & scripts
   ├─ print-runs.csv     # Log of all print runs
   └─ scripts/           # Helper scripts (renaming, exporting)
```

---

## ⚙️ Git & Git LFS Setup

This repo uses **Git Large File Storage (LFS)** for heavy binary assets.

### Install Git LFS

```bash
brew install git-lfs   # macOS
# or use your OS package manager

git lfs install
```

### Track Design Files

```bash
git lfs track "*.psd" "*.ai" "*.indd" "*.pdf" "*.png" "*.jpg"
git add .gitattributes
git commit -m "chore: track design binaries with LFS"
```

---

## 📝 Workflow

1. **Branch per concept** – e.g., `concept/navy`, `concept/mono`
2. **Work in `/src/`** – commit `.ai`/`.psd` working files
3. **Export to `/exports/`** – commit print-ready PDFs and PNGs
4. **Proofs in `/proofs/`** – low-res versions for quick review
5. **Tag approved runs** – e.g., `v1.0-card-2025-10-01`
6. **Log in `/ops/print-runs.csv`** – track vendor, stock, qty, file

---

## 🖨️ Print Notes

Each project (e.g., business cards, signage) has a `notes.md` file with:

* Vendor & order link
* Size, bleed, safe area
* Color profile (CMYK/ICC)
* Paper stock & finish
* Date, quantity, approval
* File used for print

---

## 🏷️ Naming Conventions

* **Working files (src):** `duma-card_A_v03.ai`
* **Exports:** `duma-card_v1.0_print.pdf` / `duma-card_v1.0_web.png`
* **Branches:** `concept/navy`, `tweak/qr-spacing`
* **Tags:** `v1.0-card-2025-10-01`

---

## 🚀 Usage

Clone and set up LFS before working:

```bash
git clone <repo-url>
cd dumarealty-branding
git lfs install
```

When starting a new design:

```bash
git checkout -b concept/new-idea
```

When finalizing a print run:

```bash
git tag -a v1.0-card-2025-10-01 -m "First print run"
git push --tags
```

---

## 📌 Notes

* **Fonts:** Only include licenses/specimens if redistribution is restricted.
* **SVG preferred:** Use vector exports for web where possible.
* **Binary bloat:** Archive legacy print zips outside the repo if storage/bandwidth becomes an issue.

---

## 📄 License

Internal use only – Duma Realty Inc. branding materials. Not for public redistribution.
