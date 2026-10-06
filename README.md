# Automatizaciones con IA en n8n

Workflows de n8n con agentes de IA, RAG e integraciones, construidos y probados en mi instancia autoalojada (VPS con Easypanel, Postgres y Redis).

| # | Proyecto | Qué demuestra |
|---|---|---|
| 01 | [Agente RAG multimodal con memoria](./01-agente-rag-multimodal-telegram) | RAG con Supabase/pgvector, pipeline de ingesta, texto + voz + imagen, buffer de mensajes en Redis, guardarraíles, salida estructurada |
| 02 | [Atención al cliente por WhatsApp](./02-atencion-cliente-whatsapp) | Twilio, enrutado por tipo de mensaje, transcripción de voz, guardarraíles, memoria en Postgres |
| 03 | [Facturas por voz o texto](./03-facturas-por-voz-telegram) | Extracción de datos con IA, Google Sheets + Docs + Drive, generación y envío de PDF |

## Cómo importar un workflow

1. En n8n: **Workflows → Import from file** y elige el `workflow.json` de la carpeta.
2. Asigna tus credenciales en cada nodo (OpenAI, Telegram, Supabase, Postgres, Redis, Twilio o Google, según el caso).
3. Sustituye los valores marcados como `TU_...` (IDs de archivos de Drive, número de Twilio, etc.).

Los workflows no incluyen credenciales, URLs de webhook ni IDs de mis archivos.

## Stack

n8n · OpenAI (GPT, Whisper, visión, embeddings) · Supabase (pgvector) · PostgreSQL · Redis · Telegram · Twilio · Google Workspace

---

**Oscar Navarro Viader** · [LinkedIn](https://linkedin.com/in/oscar-navarro-viader) · [ReseñIA](https://github.com/oscarviader-prog/Rese-IA)
