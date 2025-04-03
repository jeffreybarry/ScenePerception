# ScenePerception Benchmark Suite: Evaluation Guide  
**Evaluating how AI models render scenes—in images, video, and 3D space.**  

---

## 🧠 Purpose  
This guide provides a standardized method for evaluating AI-generated images in the *ScenePerception* benchmark. Each prompt is assessed according to five foundational categories:  

1. **Text Rendering & Integration**  
2. **Compositional Coherence**  
3. **Semantic Grounding**  
4. **Character Consistency & Expression**  
5. **Realism vs. Stylization Control**  

---

## 🔍 Evaluation Process  

For each generated image, evaluate the output on a scale of **0 to 5** for each criterion within the category.  

- **0** - Unacceptable: The image fails to meet any part of the criterion.  
- **1** - Poor: Significant flaws or inconsistencies.  
- **2** - Fair: Noticeable issues but partially meets the criterion.  
- **3** - Good: Meets most aspects with minor inconsistencies.  
- **4** - Very Good: Accurate and consistent, with negligible flaws.  
- **5** - Excellent: Perfect execution with no discernible issues.  

---

## 📝 1. Text Rendering & Integration  
Assesses the model’s ability to render clear and contextually accurate text within the image.  

**Evaluation Criteria:**  
- **Legibility:** Clarity and readability of the text.  
- **Contextual Accuracy:** The text appears in logical places within the scene.  
- **Stylistic Consistency:** The font, size, and style match the visual context.  

**Scoring Example:**  
- Legibility: 4  
- Contextual Accuracy: 5  
- Stylistic Consistency: 3  
- **Total: 12/15**  

---

## 🏗️ 2. Compositional Coherence  
Evaluates spatial logic, layering, and how elements are organized within the scene.  

**Evaluation Criteria:**  
- **Spatial Accuracy:** Objects appear in positions consistent with perspective and scale.  
- **Layering & Depth:** Proper foreground, midground, and background arrangement.  
- **Object Relationships:** Logical and intentional placement of interacting elements.  

**Scoring Example:**  
- Spatial Accuracy: 5  
- Layering & Depth: 4  
- Object Relationships: 4  
- **Total: 13/15**  

---

## 🧠 3. Semantic Grounding  
Assesses how accurately the image reflects the abstract ideas and concepts from the prompt.  

**Evaluation Criteria:**  
- **Concept Fidelity:** The scene accurately reflects the prompt’s abstract or concrete idea.  
- **Symbolic Accuracy:** Visual symbols match the intended representation.  
- **Coherence:** The entire scene logically aligns with the intended meaning.  

**Scoring Example:**  
- Concept Fidelity: 4  
- Symbolic Accuracy: 3  
- Coherence: 5  
- **Total: 12/15**  

---

## 🎭 4. Character Consistency & Expression  
Evaluates character appearance, posture, emotions, and interactions.  

**Evaluation Criteria:**  
- **Appearance Accuracy:** Characters match the prompt description (age, hairstyle, attire).  
- **Emotional Expression:** Characters convey emotions as specified.  
- **Interaction Logic:** Characters are positioned and posed logically relative to one another.  

**Scoring Example:**  
- Appearance Accuracy: 5  
- Emotional Expression: 4  
- Interaction Logic: 3  
- **Total: 12/15**  

---

## 🎨 5. Realism vs. Stylization Control  
Measures how well the model balances photorealism or stylization as specified.  

**Evaluation Criteria:**  
- **Stylistic Fidelity:** The chosen style matches the prompt (e.g., photorealistic, illustrative).  
- **Visual Consistency:** The image maintains a consistent stylistic tone throughout.  
- **Quality of Details:** Fine details are consistent with the chosen style.  

**Scoring Example:**  
- Stylistic Fidelity: 5  
- Visual Consistency: 4  
- Quality of Details: 5  
- **Total: 14/15**  

---

## 🗳️ Final Scoring and Reporting  
- **Category Total:** Add the scores from each criterion.  
- **Benchmark Total:** Sum of all category totals (out of 75).  
- **Report Format:**  
  ```json
  {
    "id": "T1-001",
    "model": "Midjourney",
    "date": "2025-04-03",
    "scores": {
      "text_rendering": 12,
      "compositional_coherence": 13,
      "semantic_grounding": 12,
      "character_consistency": 12,
      "realism_control": 14
    },
    "total": 63,
    "notes": "Excellent text integration, minor inconsistency in character interaction."
  }
