# BajaNet Website Revamp Plan

Revamp the BajaNet landing page from its current dark theme to an elegant, luminous light/cream aesthetic. The project will maintain a pure HTML/CSS/JS stack, implement bilingual support (ES/EN), move the privacy policy to a separate page, and refine content and branding.

## User Review Required

> [!IMPORTANT]
> The current site uses a dark theme (Black/Orange/Gold). The revamp will transition to a **Cream/White/Luminous** aesthetic. While maintaining the orange/gold accents, the primary background will be warm off-white/cream to convey a "premium" feel.

> [!NOTE]
> The multilingual support will be implemented using a simple JS-based internationalization (i18n) system using `data-i18n` attributes.

## Proposed Changes

### Core Aesthetic & UI Design
Using the `frontend-design` and `design-system` skills:
- **Visual Direction**: Luxury/Editorial. High focus on typography, generous whitespace, and subtle depth.
- **Color Palette**:
  - Primary Background: `#FAF9F6` (Cream/Off-white)
  - Secondary Background: `#F5F2ED` (Warm Cream)
  - Primary Text: `#1A1510` (Soft Black)
  - Accents: Retain refined versions of the existing Orange and Gold for continuity.
- **Typography**: Enhance the use of *Outfit* (Sans) for modern reliability and *Crimson Pro* (Serif) for editorial elegance.

---

### [Component Name] Global Refactor

#### [MODIFY] [bajanet_index.html](file:///c:/Users/Serge/Documents/Vide%20Coding%20Projects/bajanet/BajaNet/bajanet_index.html)
- **Theme Shift**: Invert CSS variables for light theme. Replace dark backgrounds with luminous cream tones and dark text.
- **Logo Update**: Replace the existing Base64 embedded logo with the relative path to `bajanet-logo.png`.
- **Multilingual Support**:
  - Add a language toggle (ES/EN) in the header to the right of the "Contactanos" button.
  - Wrap translatable text in `data-i18n` attributes.
  - Implement a `script` at the bottom to handle the translation logic.
- **Services Section**: Remove the "Cotizar" (Quote) buttons from each service item.
- **Privacy Section**: Remove the inline privacy content and replace with a link in the footer to the new page.
- **Content Synthesis**: Using `brand-voice` and `content-engine` principles, clean up and synthesize the marketing copy to be more concise and "premium."

#### [NEW] [privacy.html](file:///c:/Users/Serge/Documents/Vide%20Coding%20Projects/bajanet/BajaNet/privacy.html)
- Create a standalone page for the Privacy Policy.
- Match the new luminous/cream design system.
- Include a "Back to Home" button.

---

### Implementation Details (Skills Integration)

- **`frontend-design`**: I will use the "Frame the interface first" workflow.
  - *Tone*: Professional, Luminous, High-End.
  - *Hierarchy*: Use `Crimson Pro` for display headlines and `Outfit` for body to create an editorial look.
- **`brand-voice`**: I will extract the core message of BajaNet (reliability, local connectivity, premium service) and synthesize the current long paragraphs into punchy, high-impact statements.
- **`design-system`**: I will define a clear set of tokens for the new light theme.

## Verification Plan

### Automated Tests
- I will use the browser tool to verify the visual appearance on both Desktop and Mobile.
- I will verify the language toggle functionality (switching between ES and EN).
- I will check that all links (especially the new Privacy page) are functional.

### Manual Verification
- Verify that the "Cotizar" buttons are removed from all service entries.
- Confirm the new logo displays correctly.
- Review the synthesized content for tone and clarity.
