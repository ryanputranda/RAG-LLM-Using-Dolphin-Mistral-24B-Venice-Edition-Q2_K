# RAG-LLM-Using-Dolphin-Mistral-24B-Venice-Edition-Q2_K

Minichatbot berbasis Retrieval-Augmented Generation (RAG) untuk menjawab pertanyaan dari PDF menggunakan FAISS + LLM.

---

## Ringkasan Komponen

| Komponen   | Nilai                                                   |
|------------|---------------------------------------------------------|
| LLM        | Dolphin-Mistral-24B-Venice-Edition-Q2_K.gguf            |
| Loader     | llama-cpp-python                                        |
| n_ctx      | 4096                                                    |
| n_gpu_layers | 10                                                    |
| Embedding  | all-MiniLM-L6-v2                                        |
| Vektor DB  | FAISS IndexFlatL2                                       |
| Chunking   | size=500, overlap=100                                   |
| Retrieve   | top-k=3                                                 |
| Inferensi  | max_tokens=300, temperature=0.2, stop=</s>              |

---

Note:
Ini merupakan model RAG LLM minimimalis, proses inferencenya bisa memakan waktu hingga 20-50 menit, perlu ganti model LLM yang lebih recommended
