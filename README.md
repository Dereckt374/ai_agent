# ai_agent

Résumé rapide du script 

- Scraping → On récupère des articles sur la F1
- Chunking → On découpe le texte en morceaux
- Embedding → On transforme le texte en nombres
    - Transformer chaque morceau de texte en embedding (vecteur de nombres).
    - Stocker ces embeddings dans FAISS, une base de données rapide pour la recherche de similarité.
    - Lorsqu'une question est posée, générer son embedding et chercher les morceaux les plus proches.
- Stockage → On met tout dans une base vectorielle
- Recherche → On compare une question avec les textes stockés
- Génération de réponse → Un LLM utilise les résultats pour répondre

> See agent_test.ipynb

---

Améliorations possibles :

- Utiliser Scrapy pour un scraping plus avancé 
- Remplacer OpenAI par un LLM open-source (ex : mistral-7B, Llama 3) 
- Stocker les données dans une base vectorielle cloud (ex : Pinecone, Weaviate) 

---

