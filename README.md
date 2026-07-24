# Mobile E-Commerce UI Micro-Element Segmentation: Computer Vision & UX Audit 📱🛒

[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717?style=flat&logo=github)](https://github.com/mnkyalo/Mobile-ECommerce-UI-Micro-Element-Segmentation)
[![Format](https://img.shields.io/badge/Data_Format-Label_Studio_Polygons-blue)](#)
[![Domain](https://img.shields.io/badge/Domain-Computer_Vision_%2F_E--Commerce_UX-green)](#)

## Overview
This technical case study documents high-precision polygon segmentation on perspective-warped, skewed mobile device screens. Built with **Label Studio**, this pipeline defines a multi-class interaction taxonomy to isolate conversion-critical UI elements (such as CTAs, pricing tags, and trust badges) on high-density grid interfaces (e.g., retail marketplaces).

---

## Key Features & Dataset Specs
* **Evaluator:** Margaret Kyalo
* **Tooling:** Label Studio (Polygon Vector Masking)
* **Perspective Compensation:** Handles $34^\circ$ device roll and tilt using flexible polygon boundaries instead of rigid bounding boxes.
* **Nested Architecture:** Accommodates overlapping data tokens (e.g., interactive nodes embedded inside structural product containers).
* **Primary Objective:** Generate high-fidelity baseline data for computer vision models automated for UX conversion tracking, UI design system compliance, and competitive retail analysis.

---

## Entity Taxonomy

| Label | Color Code | Purpose & Technical Scope |
| :--- | :--- | :--- |
| **`Product_Card`** | `#FFD700` | Isolates the structural grid container housing individual consumer items. Defines spatial grid compliance. |
| **`Product_Thumbnail`** | `#FF69B4` | Extracts primary image assets of items for visual performance and styling evaluations. |
| **`Price_Tag`** | `#00BFFF` | Identifies currency placements, standard prices, and sale text for OCR text-mapping pipelines. |
| **`Search_Filter_Bar`** | `#32CD32` | Tracks top navigation arrays, including search bars, sorting chips, and filter inputs. |
| **`Add_To_Cart_Button`** | `#00F5FF` | Maps primary actionable CTA targets (e.g., grid cart buttons and floating global elements). |
| **`Trust_Review_Badge`** | `#FF4500` | Isolates review scores, social proof metrics (e.g., "905 sold"), and shipping badges for CRO models. |
| **`Device_Frame`** | `#8A2BE2` | Tracks physical hardware chassis curves to isolate display content from real-world backgrounds. |

---

## Workspace Screenshot

![Label Studio Interface](assets/label_studio_ui.png)
*Figure 1: High-density polygon annotation capturing micro-elements on a perspective-warped mobile display in Label Studio.*

---

## Production Impact
By converting complex, unconstrained physical device captures into structured UI spatial metadata, this dataset bridges the gap between raw pixel streams and automated e-commerce business intelligence.
