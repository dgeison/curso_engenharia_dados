# ⚠️ IMPORTANTE: Configuração de Chaves de API

Este diretório contém notebooks que utilizam APIs externas (principalmente OpenAI). Para usar estes notebooks, você precisa configurar suas chaves de API de forma segura.

## 🔐 Como Configurar

### Opção 1: Variáveis de Ambiente (Recomendado)
```bash
export OPENAI_API_KEY="sua_chave_aqui"
```

### Opção 2: Arquivo .env
1. Copie o arquivo `.env.example` para `.env`
2. Configure suas chaves no arquivo `.env`
3. Use `python-dotenv` para carregar:
```python
from dotenv import load_dotenv
load_dotenv()
```

### Opção 3: Substituição Direta
Substitua `YOUR_API_KEY_HERE` pela sua chave nos notebooks (não recomendado para repositórios públicos).

## 🚫 O que NÃO fazer

- ❌ Nunca commite chaves de API no git
- ❌ Nunca compartilhe chaves em screenshots
- ❌ Nunca use chaves em código de produção sem criptografia

## 📚 Notebooks Afetados

- `3.GPT.ipynb` - Introdução ao GPT
- `AgenteRAGEspecializado.ipynb` - Agente RAG especializado

## 🆘 Obtendo Chaves de API

- **OpenAI**: https://platform.openai.com/api-keys
- **Hugging Face**: https://huggingface.co/settings/tokens
- **LangChain**: https://smith.langchain.com/

---
*Lembre-se: Segurança em primeiro lugar! 🔒*