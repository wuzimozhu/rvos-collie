# RVOS-CoLLIE

RVOS-CoLLIE is a novel dataset designed for **Referring Video Object Segmentation** (RVOS) with **CoLLIE-style implicit linguistic expressions** and **logical reasoning** enhancements.

## 🧠 Highlights

- 💬 Implicit, colloquial, and logically-grounded language expressions.
- 🎥 Based on Ref-YouTube-VOS video segmentation data.
- 🧪 Includes a sample subset: `rvos_collie_val_sample.json` for quick testing.

## 📁 Dataset Structure
RVOS-CoLLIE/
├── Annotations.zip # Segmentation masks in PNG format  
├── JPEGImages.zip # RGB frames of videos  
├── rvos_collie_val_sample.json # A small val subset with implicit queries  
└── README.md  


## 🔍 File Description

- `Annotations.zip`: contains the segmentation masks, organized by video/frame/object.
- `JPEGImages.zip`: original frames extracted from Ref-Youtube-VOS videos.
- `rvos_collie_val_sample.json`: includes a small subset of videos with expressions in this format:
```json
{
  "videos": {
    "video_id": {
      "expressions": {
        "0": {
          "exp": "explicit expression",
          "imp": "implicit expression",
          "logic_fop": "∃x (...)",
          "logic": "logic reasoning expression",
          ...
        },
        ...
      },
      ...
    }
  }
}


