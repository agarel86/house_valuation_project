# House Perceptual Attribute Rating Tool

Interactive tool for validating and rating AI-generated perceptual attributes
of residential houses, as described in:

> **From Vision to Prediction: A Multimodal-AI Pipeline to Generate
> Perceptual Attributes for Price Prediction**

## How to use

1. Open the GitHub Pages site (or open `index.html` locally via a server)
2. **Tab 1 – Validate Taxonomy**: Review each variable's definition and rationale; indicate whether it matters for house valuation and whether you agree with its first/second order classification
3. **Tab 2 – Validate AI Grades**: For a specific house, review photos and confirm/reject the AI's grades
4. **Tab 3 – Rate Houses**: Independently grade each perceptual attribute from photos
5. Export your results as JSON or CSV when done

## Quick local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Data

- **44 houses** with listing photographs
- **59 perceptual attributes** per house (where AI features are available)
- Attributes classified as **first-order** or **second-order**
- Organized into 3 sections: Property Appeal, Environmental Cues, Staging & Presentation

## Rating scale

| Grade     | Meaning                                    |
|-----------|--------------------------------------------|
| Excellent | Top quality, no visible issues              |
| Good      | Above average, minor imperfections          |
| Average   | Typical, neither notably good nor bad       |
| Bad       | Below average, visible problems             |
| Terrible  | Severe issues, major defects                |
| Unknown   | Cannot be assessed from available photos    |

All progress is saved automatically in your browser's local storage.
