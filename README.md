# 大荒雜貨鋪：郭掌櫃的山海經配貨 RAG

客官帶著現代煩惱上門，郭掌櫃翻開《山海經》替你配貨：每件貨都引用原文、附上出處與風險，帳冊上沒有的東西就老實說查無此物。

生成式 AI 課程作業，程式以 [yenlung/Generative-AI](https://github.com/yenlung/Generative-AI) 的 RAG 範例為基底，並由 Claude Code 協助修改。

| 檔案 | 內容 |
|---|---|
| `RAG01_shanhai_build.ipynb` | 讀取語料、向量化、建立 FAISS 索引、檢索評估，輸出 `rag-data.zip` |
| `RAG02_shanhai_chatbot.ipynb` | 下載 `rag-data.zip`，以 Gradio 提供 RAG 對話機器人 |
| `shanhai-source.zip` | 869 個條目的 TXT 語料 |
| `rag-data.zip` | 向量資料庫 |

## 資料來源

《山海經》18 卷取自[維基文庫](https://zh.wikisource.org/wiki/山海經)（公有領域），每個條目記錄 revision。原文未改寫，僅依《四部叢刊》本校正 7 處明顯衍字與錯字，清單見語料內的 `corrections.json`。

內容為神話傳說，不是醫療建議，請勿照著吃。
