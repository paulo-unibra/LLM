# Mini ChatGPT com Chain of Thought

Um chat demo que mostra o raciocínio do modelo (chain of thought) antes de apresentar a resposta final.

## � Versões Disponíveis

### 🎓 Versão para Apresentação Acadêmica (RECOMENDADO PARA FACULDADE)

#### ⭐ **`chat_apresentacao.html`** - Demo Educacional
**PERFEITO PARA SUA APRESENTAÇÃO!**
- 🎯 Layout dividido: Chat (esquerda) + Bastidores Técnicos (direita)
- 📚 Mostra todas as 6 etapas do processamento em tempo real
- 🔤 Visualização de tokenização
- 🧮 **NOVO: Cálculos matemáticos REAIS:**
  - Embeddings: Vetores de 4D (simula os 12.288D do GPT)
  - Mecanismo de Atenção: Matriz 3x3 com pesos reais
  - Softmax: Distribuição de probabilidades
- ⚙️ Explicação técnica do processamento neural
- 💡 5 perguntas pré-programadas sobre IA/LLM
- ✏️ **NOVO: Digite qualquer pergunta!**
- ✅ **Não precisa de API Key** (simulação offline)
- 🎬 Ideal para demonstrações em aula
- 🌑 Tema dark para melhor visibilidade em projetor

### 🌐 Versões HTML com OpenAI API Real

#### 🔹 Versão Completa (`chat.html`)
Interface web moderna com:
- Design gradient e animações suaves
- Histórico de conversas expansível
- Seleção de modelo (GPT-3.5, GPT-4)
- Controle de temperatura
- Armazenamento local da API Key
- Layout responsivo

#### 🔹 Versão Simples (`chat_simples.html`)
Interface minimalista e direta, ideal para demonstrações rápidas.

### 🐍 Versões Python/Streamlit

#### 🔹 Versão Básica (`chat_demo.py`)
Interface simples e direta, ideal para demonstrações rápidas.

#### 🔹 Versão Pro (`chat_demo_pro.py`)
Interface avançada com:
- Histórico de conversas
- Seleção de modelo (GPT-3.5, GPT-4, etc.)
- Controle de temperatura
- Ajuste de velocidade de exibição
- Layout expandido

## 🚀 Como Usar

### 🎓 Para Apresentação Acadêmica (Mais Rápido!)

**Arquivo: `chat_apresentacao.html`**

1. **Abra o arquivo:**
   - Dê um duplo clique em `chat_apresentacao.html`
   - Abre direto no navegador

2. **Durante a apresentação:**
   - Lado esquerdo = Interface do usuário
   - Lado direito = Bastidores técnicos
   - **Opção 1:** Clique nas perguntas pré-programadas
   - **Opção 2:** Digite qualquer pergunta no campo de texto
   - Veja as 6 etapas do processamento acontecendo:
     1. Recepção do Input
     2. Tokenização (divisão em pedaços)
     2.5. **Embeddings (NOVO!)** - Vetores numéricos reais
     3. Processamento Neural
     3.5. **Mecanismo de Atenção (NOVO!)** - Matriz de atenção
     4. Geração da Resposta
     4.5. **Softmax (NOVO!)** - Probabilidades de tokens
     5. Resumo Final com contagem de operações

3. **Vantagens:**
   - ✅ Não precisa de API Key
   - ✅ Funciona 100% offline
   - ✅ Demonstração visual e didática
   - ✅ 5 perguntas sobre IA/LLM prontas
   - ✅ **Aceita qualquer pergunta digitada!**
   - ✅ Mostra tokens, processamento, métricas
   - ✅ **Exibe cálculos matemáticos reais** (embeddings, atenção, softmax)
   - ✅ Tema dark para projeção

📖 **Veja o arquivo `GUIA_APRESENTACAO.txt` para roteiro completo!**

---

### Versão HTML (Mais Fácil) ✨

**Não precisa instalar nada!** Apenas abra o arquivo HTML no navegador:

1. **Abra o arquivo:**
   - Dê um duplo clique em `chat.html` (versão completa)
   - OU `chat_simples.html` (versão minimalista)

2. **Configure a API Key:**
   - Cole sua OpenAI API Key no campo indicado
   - A chave será salva localmente no navegador

3. **Use:**
   - Digite sua pergunta
   - Clique em "Processar"
   - Veja o raciocínio aparecer passo a passo
   - Veja a resposta final

**Dica:** Funciona em qualquer navegador moderno (Chrome, Firefox, Edge, Safari)

---

---

### Versão Python/Streamlit

**1. Instalar dependências:**
```bash
pip install -r requirements.txt
```

**2. Configurar OpenAI API Key:**

Você pode configurar a API Key de duas formas:

**Opção A: Variável de ambiente**
```bash
export OPENAI_API_KEY='sua-api-key-aqui'
```

**Opção B: Interface do Streamlit**
- Digite a API Key diretamente na barra lateral do aplicativo

**3. Executar o aplicativo:**

Versão Básica:
```bash
streamlit run chat_demo.py
```

Versão Pro:
```bash
streamlit run chat_demo_pro.py
```

O aplicativo abrirá automaticamente no seu navegador em `http://localhost:8501`

---

## 🎯 Qual Versão Usar?

| Característica | **Apresentação** | HTML c/ API | Python/Streamlit |
|----------------|------------------|-------------|------------------|
| **Instalação** | ✅✅✅ Nenhuma | ✅ Nenhuma | ❌ Requer pip install |
| **API Key** | ✅✅✅ Não precisa | ❌ Precisa OpenAI | ❌ Precisa OpenAI |
| **Internet** | ✅✅✅ Offline | ⚠️ Precisa para API | ⚠️ Precisa para API |
| **Educacional** | ✅✅✅ Perfeito! | ❌ Só chat | ⚠️ Só chat |
| **Visualização** | ✅✅✅ Mostra bastidores | ❌ Não | ❌ Não |
| **Para Aula** | ✅✅✅ Ideal | ⚠️ OK | ⚠️ OK |
| **Respostas Reais** | ❌ Simuladas | ✅ OpenAI real | ✅ OpenAI real |

**Recomendação para Apresentação Acadêmica:** Use `chat_apresentacao.html` 🎓  
**Recomendação para Uso Real:** Use `chat.html` com OpenAI API 💬

## 📝 Funcionalidades

- **Campo de Pergunta**: Digite qualquer pergunta
- **Raciocínio do Modelo**: Visualize o processo de pensamento passo a passo
- **Resposta Final**: Veja a resposta concisa baseada no raciocínio
- **Efeitos Visuais**: Animações de "pensamento" e "digitação" para tornar a demo mais interessante

## 💡 Exemplo de Uso

1. Digite uma pergunta como: "Como funciona a fotossíntese?"
2. Clique em "🚀 Processar"
3. Observe:
   - Seu pergunta sendo exibida
   - O raciocínio aparecendo passo a passo
   - A resposta final sendo "digitada"

## ⚙️ Tecnologias

- **Streamlit**: Interface web interativa
- **OpenAI API**: Geração de texto com GPT-3.5-turbo
- **Python 3.8+**: Linguagem de programação

## 📌 Notas

- Requer uma API Key válida da OpenAI
- Consome créditos da sua conta OpenAI a cada pergunta
- Usa o modelo `gpt-3.5-turbo` por padrão
