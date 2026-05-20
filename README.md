# 💰 FinanCIA - Organizador Financeiro Pessoal com IA

## 📱 Sobre o Projeto

**FinanCIA** é um aplicativo de finanças pessoais desenvolvido como parte do desafio do curso de IA, utilizando a abordagem de **Vibe Coding** no Google AI Studio.

A proposta é simples: **controlar suas finanças por meio de uma conversa natural**, sem planilhas complicadas ou formulários manuais. O app conta com um agente financeiro amigável chamado **FinanCIA** que ajuda o usuário a registrar gastos, definir metas e acompanhar hábitos financeiros de forma leve e descomplicada.

---

## ✨ Funcionalidades Implementadas (validadas em teste)

| Funcionalidade | Status | Detalhe |
|----------------|--------|---------|
| 💬 **Chat inteligente** | ✅ 100% | Responde perguntas sobre metas, economia e finanças pessoais |
| 🍔 **Menu de categorias** | ✅ 100% | 6 botões: Alimentação, Lazer, Contas, Investimentos, Transporte, Outros |
| 📊 **Painel de gastos dinâmico** | ✅ 100% | Atualiza em tempo real ao registrar gastos |
| 🎯 **Metas de economia** | ✅ 100% | Ex: "Meta: Visitar a Disney em 6 meses com R$20 mil" |
| 🤖 **Agente FinanCIA** | ✅ 100% | Tom amigável, encorajador, responde com dicas práticas |
| 📈 **Gráficos por categoria** | ✅ 100% | Mostra corretamente os valores em cada categoria |
| 🔄 **Integração menu + painel** | ✅ 100% | Clique no botão → digita valor → painel atualiza |

### ⚠️ Limitação conhecida

Perguntas específicas sobre **"bolsa de valores"** ou **"investimentos complexos"** podem retornar erro 503 devido à alta demanda no modelo Gemini (problema nos servidores do Google, não no código do app). Perguntas sobre metas, economia pessoal e registro de gastos funcionam normalmente.

---

## 🛠️ Tecnologias e Ferramentas

- **React + Tailwind CSS** – Interface do usuário
- **Firebase Firestore** – Banco de dados
- **Google AI Studio (Agente Antigravity)** – Desenvolvimento via Vibe Coding

### Por que Google AI Studio em vez de Lovable?

O Lovable gratuito permite apenas **5 interações por dia**, inviabilizando um desenvolvimento completo. Optei pelo **Google AI Studio**, que oferece cota generosa, modo Build com prévia ao vivo e deploy gratuito.

---

## 🎮 Como Usar (demonstrado no vídeo)

### Registrar gastos via menu de categorias
1. Clique em qualquer botão (ex: 🍔 Alimentação)
2. Digite o valor quando o app perguntar
3. O gasto é registrado e o painel atualiza automaticamente

### Definir metas de economia
Digite no chat algo como:  
*"Meta: Visitar a Disney em 6 meses com R$20 mil"*

A FinanCIA responde com:
- Cálculo do valor necessário por mês
- Dicas para otimizar o orçamento
- Confirmação do registro da meta

### Fazer perguntas financeiras
Digite perguntas como:  
*"Me dê dicas para economizar dinheiro"*

A FinanCIA responde com dicas práticas e encorajadoras.

---

## 📸 Prints e Vídeo de Demonstração

*(Insira aqui os prints do seu app e o link do vídeo de demonstração)*

### O que o vídeo mostra:
- Tela inicial com menu de 6 categorias e mensagem de boas-vindas
- Teste de todas as categorias (cada uma pede o valor e registra)
- Definição de meta financeira (Disney, 6 meses, R$20 mil)
- Resposta completa da FinanCIA com planejamento mensal
- Painel de gastos atualizando em tempo real
- Gráficos mostrando valores nas categorias corretas

---

## 🧠 Processo de Desenvolvimento

### Prompt final utilizado
