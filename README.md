### Wdrażanie AI i automatyzacji · n8n · RAG · agenci AI · modele lokalne

Buduję z narzędzi AI systemy, które pracują codziennie i same raportują mi na Telegramie. Z agentami pracuję jak z zespołem: projektuję, zlecam, sprawdzam i dowożę. Kod piszą agenci, ja odpowiadam za to, żeby całość działała, a liczby sprawdza skrypt, nie model.

**Co działa teraz**

- **[aipoc-lab](https://aipoclab.creativeaidrivenpm.com)**: blog, który codziennie od 4:00 do 9:00 czyta 15 źródeł i przygotowuje newsy dnia w czterech językach (PL, EN, DE, ZH). Czat AI na RAG (PostgreSQL + pgvector) przeszedł 548 prób ataku bez wycieku danych. Codziennie skrypt w Pythonie składa rolkę z mapy bazy wektorowej, bramka sprawdza liczby, a publikacja rusza po moim przycisku na Telegramie.
- **Automatyzacje i serwery:** 117 workflowów w n8n (37 działa stale) i zadania cron na dwóch serwerach w sieci Tailscale. Agent serwera zgłasza awarie, codzienny raport sprawdza kopie, dysk i podatności, a raport z Google Search Console przychodzi co tydzień. Kopie 3-2-1, okna serwisowe, runbooki z realnych awarii.
- **Persona AI**, która sama prowadzi swoje social media: na polecenie z Telegramu korzysta z Google Trends, wiadomości i wiedzy z labu, a rolki i karuzele renderuje silnik Auto Reels przez API.
- **Modele lokalne:** Ollama na serwerze i Qwen 27B na własnej karcie GPU, testowane pod zadania nocne.

**Otwarte i za darmo**

- [fiszka](https://github.com/ch3sh1r3xx11/fiszka): moja mała sieć neuronowa (252 194 parametry), która rozpoznaje 17 tematów AI w tekstach; model na [Hugging Face](https://huggingface.co/aipoc-lab/fiszka) i [zbiór 9 968 opisanych tekstów](https://huggingface.co/datasets/aipoc-lab/fiszka-dataset), [podgląd na żywo](https://aipoclab.creativeaidrivenpm.com/fiszka)
- [fiszka-dekoder-instagram](https://github.com/ch3sh1r3xx11/fiszka-dekoder-instagram): cały model wrzucony na Instagram w 6 zrzutach ekranu i dekoder, który odtwarza go ze screenshotów
- [paos_workflow_00_11](https://github.com/ch3sh1r3xx11/paos_workflow_00_11): mój system pracy z plikami projektu i skill /praca, który daje agentom AI ciągłość kontekstu między sesjami
- [cheshire-companion](https://github.com/ch3sh1r3xx11/cheshire-companion): agent AI na pulpit Windows (Gemini albo Ollama) z pamięcią i wzrokiem, z piaskownicą i strażnikiem komend
- [domowy-serwer-ai](https://github.com/ch3sh1r3xx11/domowy-serwer-ai): podręcznik, jak postawić serwer AI 24/7 ze starego komputera biurowego

**Narzędzia:** n8n · Claude Code · Gemini API · OpenRouter · Ollama · PyTorch · PostgreSQL + pgvector · Docker · Tailscale · Cloudflare (Workers, R2, tunel) · Telegram Bot API · Google Search Console API · Buffer API · Hugging Face

[blog](https://aipoclab.creativeaidrivenpm.com) · [Credly](https://www.credly.com/users/mateusz-polomski) · [LinkedIn](https://www.linkedin.com/in/mateusz-polomski-ai)

---

*Building AI systems with agents and keeping them running in production: n8n (117 workflows), RAG, Telegram agents with approval buttons, local models, two self-hosted servers. Open models and datasets on Hugging Face. Based in Poland, open to remote work.*
