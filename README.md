# Organ Mountain Outfitters (OMO) — Multicam Editorial & Color Grade

An industry-standard multi-camera documentary and commercial brand profile produced in **DaVinci Resolve 21**. This repository contains the complete DaVinci Resolve Project Archive (`.dra`), structural metadata, project database (`project.drp`), and synchronized multi-track media files managed via Git Large File Storage (Git LFS).

---

## Deliverables & Links

* **Stream / Master Preview (YouTube Unlisted):** `[INSERT YOUR YOUTUBE/STREAMING LINK HERE]`
* **Full Production Archive (.dra):** Available directly within this repository via Git LFS clone, or packaged as `OMO INTERVIEW.dra.zip`.
* **Editor & Colorist:** Pulak Saha
* **Primary NLE & Grading Suite:** DaVinci Resolve 21

---

## Technical Overview & Workflow

### 1. Multi-Camera Ingestion & Waveform Synchronization
* **Media Alignment:** Synchronized three independent camera angles (A-Cam wide interview, B-Cam medium close-up, C-Cam workshop detail) using automated audio waveform phase matching.
* **Angle Switching & Trimming:** Conducted dynamic real-time angle switching via the Angle Viewer; refined narrative pacing and eye-trace across soundbites using Roll and Slip dynamic trimming tools.
* **Pacing & Transitions:** Utilized J-cuts and L-cuts to lead audio transitions naturally between conversational dialogue and cutaway B-roll actions.

### 2. Color Management & Shot-to-Shot Matching
* **Color Pipeline:** Implemented a **DaVinci YRGB Color Managed** (RCM) workflow targeted for standard broadcast **Rec.709 / Gamma 2.4** delivery.
* **Primary Balancing:** Standardized exposure latitudes between high-contrast outdoor desert daylight and subdued indoor apparel workshop scenes using the Primary Wheels and RGB Parade monitoring.
* **Secondary Skin Isolation:** Isolated subject skin tones across all angles using 3D Qualifiers and tracked circular Power Windows, aligning hues to the Vectorscope skin-tone reference line to eliminate camera-to-camera color shifts.

### 3. Fairlight Audio Mastering
* **Dialogue Enhancement:** Extracted rumble and low-end room resonance using an 80 Hz high-pass EQ curve, followed by gentle dynamics compression for vocal consistency.
* **Loudness Standards:** Mastered dialogue and background ambience stems to the standard streaming delivery target of **-14 LUFS** (integrated loudness) with peak safety limiting.

---

## Repository Structure

```text
OMO INTERVIEW.dra/
├── project.drp              # DaVinci Resolve Project Database (timelines, grades, cuts)
├── .gitattributes           # Git LFS configuration rules
├── MediaFiles/              # Rushes and production assets tracked via LFS
│   ├── INTERVIEW/           # Synced A/B/C camera files and discrete audio takes
│   ├── B-ROLL/              # High-latitude cutaway media
│   ├── AUDIO/               # External master dialogue WAV stems
│   ├── MUSIC/               # Master soundtrack stems
│   └── SFX/                 # Foley and spot effects
└── Cache/                   # Waveform and proxy cache files
