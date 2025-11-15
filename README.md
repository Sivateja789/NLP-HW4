# NLP-HW4      

Student Info
Name: SIVA TEJA KATTA      
Student ID: 700774274        

---

## 📖 Problem Statement
Perform NLP preprocessing and entity extraction on the given input texts using **NLTK only**  
(spaCy not supported in Python 3.14).

You must implement:

### **Q1. Text Preprocessing**
- Tokenization  
- Stopword Removal  
- Lemmatization (no stemming)  
- POS Tagging → keep only **verbs** and **nouns**

### **Q2. Named Entity Recognition + Pronoun Ambiguity Detection**
- Perform NER  
- Detect pronouns: `"he"`, `"she"`, `"they"` → print a warning message

---

## 📝 Q1 — Text Preprocessing

### **Input Text**
> "John enjoys playing football while Mary loves reading books in the library."

### **Steps Performed**
1. Tokenized the sentence into word tokens  
2. Removed English stopwords  
3. Applied WordNet lemmatization  
4. Filtered tokens to keep only **verbs and nouns**  
5. Printed final processed tokens  

---

## 📝 Q2 — NER + Pronoun Ambiguity Detection

### **Input Text**
> "Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch."

### **Steps Performed**
1. Tokenized the input text  
2. Applied NLTK POS tagging  
3. Performed Named Entity Recognition (NER)  
   - PERSON  
   - ORGANIZATION  
   - GPE (Location)  
4. Checked for pronouns: **he, she, they**  
5. Printed a warning message if pronoun ambiguity detected  

---

## 📈 Results Summary

### ✔ Q1 Output  
Only **nouns and verbs** were retained after preprocessing.  
The pipeline successfully:
- removed stopwords  
- lemmatized tokens  
- extracted nouns and verbs  

---

### ✔ Q2 Output  
NER detected the following entities:

| Entity     | Type        |
|------------|-------------|
| Chris      | PERSON      |
| Alex       | PERSON      |
| Apple      | ORGANIZATION |
| California | GPE         |

Pronoun detected: **"He"**  
→ ⚠️ **Warning: Possible pronoun ambiguity detected!**

---


