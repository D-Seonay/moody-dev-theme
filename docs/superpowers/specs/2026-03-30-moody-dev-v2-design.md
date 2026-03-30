# Design Spec: Moody Dev v2 - Pixel/Lego Revamp

**Date:** 2026-03-30  
**Status:** Approved  
**Topic:** Theme Modernization & Feature Expansion

## 1. Overview
The goal of Moody Dev v2 is to modernize the visual aesthetic of the Oh My Posh theme using a "Pixel/Lego" style and expand its utility by adding comprehensive system, cloud, network, and language segments.

## 2. Visual Style: Pixel/Lego
The primary visual change is the transition from standard Powerline separators to a pixelated look.

- **Separators:** Replace `\ue0b0` () with `\ue0c6` ().
- **Secondary Prompt:** Maintain `\u2026` (…).
- **Transient Prompt:** Maintain `❯`.
- **Glyphs:** Ensure icons for new segments align with the retro-dev/pixel aesthetic (e.g., using simpler, blockier Nerd Font icons where available).

## 3. Segment Specifications

### 3.1. System Information
- **CPU:** Display usage percentage. Icon: `\ufb19` (﬙) or similar.
- **RAM:** Display usage percentage. Icon: `\uf85a` () or similar.
- **Color:** `p:accent_red`.

### 3.2. Cloud Providers
- **AWS:** Profil and Region (Existing).
- **Azure:** Display active subscription/environment. Icon: `\ufd03` (ﴃ). Color: `p:accent_blue`.
- **GCP:** Display active project/account. Icon: `\uf992` (漣). Color: `p:accent_magenta`.

### 3.3. Network
- **WiFi/IP:** Display SSID or local IP. Icon: `\uf1eb` () or `\ufb4e` (פֿ).
- **Color:** `p:accent_cyan`.

### 3.4. Languages (Extended)
- **Node:** (Existing).
- **Python:** (Existing).
- **Go:** Display version. Icon: `\ue627` (). Color: `p:accent_cyan`.
- **Rust:** Display version. Icon: `\ue7a8` (). Color: `p:accent_orange`.
- **Java:** Display version. Icon: `\ue256` (). Color: `p:accent_red`.

## 4. Layout & Architecture
The theme will be organized into two main blocks:
1.  **Primary Prompt (Left):** OS, Time, Path (Powerline), Git (Powerline), Separator Close.
2.  **Context/Language Block (Left, below or same line depending on space):** Node, Python, Go, Rust, Java, Cloud (AWS/Azure/GCP), System (CPU/RAM), Status.
3.  **Right Prompt (RPROMPT):** Spotify, Battery, Execution Time.

**New Structural Changes:**
- All Powerline segments will use the `\ue0c6` separator.
- The `text` segment used to "close" the Powerline arrow will be updated to `\ue0c6`.

## 5. Success Criteria
- [ ] All separators updated to Pixel/Lego style.
- [ ] New segments (CPU, RAM, Azure, GCP, Network, Go, Rust, Java) functional.
- [ ] Visual consistency across all segments (colors from the palette).
- [ ] No regression in existing Git or Path functionality.
