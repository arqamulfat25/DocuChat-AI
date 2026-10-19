# DocuChat-AI
DocuChat AI is a RAG-based chatbot that analyzes documents and generates summaries and key questions.
Here is what it does and how:

𝗠𝘂𝗹𝘁𝗶-𝗱𝗼𝗰𝘂𝗺𝗲𝗻𝘁 𝗖𝗵𝗮𝘁 𝘄𝗶𝘁𝗵 𝗣𝗲𝗿-𝗙𝗶𝗹𝗲 𝗖𝗼𝗻𝘁𝗿𝗼𝗹
Load PDFs, Word files, CSVs, or plain text files together in one session. Before asking anything, you can toggle which documents the model can retrieve so your answers stay scoped to what you care about.

𝗜𝗻𝗰𝗿𝗲𝗺𝗲𝗻𝘁𝗮𝗹 𝗜𝗻𝗱𝗲𝘅𝗶𝗻𝗴
Adding a new file mid-session does not rebuild the vector store. New chunks are merged directly into the existing FAISS index, keeping latency flat whether you have one file or ten loaded.

𝗚𝗿𝗼𝘂𝗻𝗱𝗲𝗱 𝗔𝗻𝘀𝘄𝗲𝗿𝘀 𝘄𝗶𝘁𝗵 𝗣𝗮𝗴𝗲-𝗟𝗲𝘃𝗲𝗹 𝗖𝗶𝘁𝗮𝘁𝗶𝗼𝗻𝘀
Every response shows the exact pages it retrieved from, with expandable excerpts. If the answer is not in the document, the model says so instead of guessing.

𝗔𝘂𝘁𝗼-𝗦𝘂𝗺𝗺𝗮𝗿𝘆 𝗮𝗻𝗱 𝗦𝘂𝗴𝗴𝗲𝘀𝘁𝗲𝗱 𝗤𝘂𝗲𝘀𝘁𝗶𝗼𝗻𝘀
When you upload a document, the system runs a semantic search across it, generates a 5-point summary, and surfaces 3 questions a reader would naturally ask. No cold-start awkwardness.

𝗖𝗼𝗻𝘃𝗲𝗿𝘀𝗮𝘁𝗶𝗼𝗻𝗮𝗹 𝗠𝗲𝗺𝗼𝗿𝘆
The last 5 exchanges stay in context, so follow-up questions resolve correctly without re-explaining what you just discussed.

𝗠𝘂𝗹𝘁𝗶-𝗙𝗼𝗿𝗺𝗮𝘁 𝗘𝘅𝗽𝗼𝗿𝘁
The full conversation exports to TXT, Markdown, or PDF, clean and ready to share or document.

Stack: Python · LangChain · HuggingFace Inference Endpoints (Zephyr-7B) · FAISS · sentence-transformers · Streamlit
