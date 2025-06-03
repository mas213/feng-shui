# 🧾 Product Requirements Document (PRD)

## Product Name: FengShuiRoom  
**Prepared By:** [Your Name]  
**Date:** [Today's Date]

---

## 1. Overview

**Goal:**  
Design a mobile/web application that helps users rearrange furniture in their rooms to align with Feng Shui principles for better energy flow, comfort, and productivity.

**Target Users:**  
- Homeowners or renters  
- Interior designers  
- People interested in wellness, harmony, and Eastern philosophy

---

## 2. Problem Statement

Most people arrange furniture without understanding the subtle effects on energy flow. Poor layouts can lead to discomfort, stress, or inefficiency. There’s no simple tool today that combines **room layout scanning** with **Feng Shui recommendations**.

---

## 3. Core Features

### A. Room Layout Input
- Upload a room photo or floor plan  
- Manual drag-and-drop room layout builder  
- AI-powered room scanner (optional: use LiDAR or ARKit for mobile devices)

### B. Furniture Identification
- Detect furniture automatically from photo (optional AI vision)  
- Or allow user to add/edit furniture items manually  
- Item types: bed, desk, chair, wardrobe, sofa, plants, etc.

### C. Feng Shui Engine
- Analyze layout based on key Feng Shui rules:
  - Command position
  - Bagua map overlay
  - Chi (energy) flow
  - Avoiding "poison arrows" and bad alignments
- Recommend optimal positioning  
- Provide a 3D or 2D rearrangement suggestion  
- Explain the rationale behind each suggestion

### D. Recommendations & Tips
- Feng Shui score (0–100) for current layout  
- Custom suggestions to improve:  
  _e.g., “Move desk to face door”, “Add mirror to reflect light”_  
- Optional enhancements:
  - Elements (wood, fire, earth, metal, water)
  - Colors
  - Lighting

### E. Save & Share Designs
- Save multiple room configurations  
- Export before/after layouts  
- Share with others via PDF, image, or link

---

## 4. Nice-to-Have Features (Future Releases)
- Augmented Reality preview  
- Personalized Feng Shui based on birth chart  
- Integration with smart home for mood lighting, scents  
- Marketplace for Feng Shui-aligned furniture

---

## 5. User Stories

| As a...        | I want to...                     | So that...                                 |
|----------------|----------------------------------|---------------------------------------------|
| Homeowner      | Scan my bedroom                 | I can see how to arrange it for better sleep |
| Designer       | Upload a client's floor plan    | I can create a Feng Shui-optimized layout   |
| Enthusiast     | See energy flow on a map        | I can balance the elements in my space      |

---

## 6. Success Metrics

- 90%+ layout scan accuracy  
- 75%+ user satisfaction with layout suggestions  
- Feng Shui scores improve on reconfiguration in 95%+ cases  
- 20%+ monthly user retention

---

## 7. Tech Stack Suggestions

- **Frontend:** React (Web), Swift/Flutter (Mobile)  
- **Backend:** Node.js + Python for Feng Shui rules engine  
- **Computer Vision:** TensorFlow/MediaPipe for layout parsing  
- **Optional:** ARKit/ARCore for spatial mapping

---
