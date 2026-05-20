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

## 📸  Vídeo de Demonstração

<img src="assets/Demonstração-FinanCIA.gif" alt="FinanCIA funcionando" width="100%">

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

[INSTRUÇÃO DE PERSONALIDADE]
Você é um consultor financeiro amigável e paciente, especializado em ajudar iniciantes. Tom de voz: encorajador, simples, sem jargões. Todos os textos em português.

[TAREFA PRINCIPAL]
Crie um aplicativo web de Organização de Finanças Pessoais com chat para registrar gastos, classificação automática, painel de gastos, menu de categorias com botões (Alimentação, Lazer, Contas, Investimentos, Transporte, Outros), e agente financeiro chamado FinanCIA. Use React, Tailwind CSS e Firebase. Tudo em português.



### Iterações realizadas

1. Geração inicial do app (chat + painel + classificação automática)
2. Correção do título (estava "calculadora")
3. Adição do menu de categorias com 6 botões
4. Integração do menu com o painel (atualização em tempo real)
5. Correção do erro de modelo desatualizado (Gemini 1.5 → 3.5 Flash)
6. Melhoria do tratamento de erros no chat

---

## 💭 Reflexão sobre o Vibe Coding

### O que funcionou bem?

O Google AI Studio gerou um app funcional com chat, menu de categorias e painel de gastos em poucas interações. A adição do menu de categorias e a integração em tempo real funcionaram perfeitamente na primeira tentativa.

O agente FinanCIA manteve o tom amigável e encorajador em todas as interações, exatamente como pedido na personalidade.

### O que não funcionou como esperado?

**Erro 503 por alta demanda:** Durante os testes, perguntas sobre "bolsa de valores" retornaram erro 503 com a mensagem "This model is currently experiencing high demand". Investiguei e descobri que:
- O erro não estava no código do app
- Era um problema nos servidores do Google (modelo Gemini 3.5 Flash Preview sobrecarregado)
- Afeta até contas pagas em momentos de pico

**Interface do Google AI Studio:** O campo "System Instructions" não estava visível, exigindo adaptação na estrutura do prompt.

### O que aprendi sobre conversar com IAs?

**1. Nem todo erro é código** – O erro 503 me ensinou a diagnosticar a camada do problema: frontend, backend ou infraestrutura. Saber quando o problema é do provedor é uma habilidade valiosa.

**2. Clareza é tudo** – Prompts estruturados com separação clara entre "personalidade do agente" e "tarefa técnica" geraram resultados muito melhores.

**3. Iterar é melhor que acertar de primeira** – Cada funcionalidade foi adicionada, testada e ajustada em ciclos rápidos.

**4. A ferramenta certa faz diferença** – Google AI Studio (cota generosa) vs Lovable (5 interações/dia). Sem essa escolha, não teria sido possível iterar até o app ficar pronto.

**5. Documentar os problemas é parte do aprendizado** – O erro 503 virou o trecho mais rico da minha reflexão, mostrando que Vibe Coding não é só sobre acertos.

---

## 🏆 Conclusão

O FinanCIA é um aplicativo funcional que prova ser possível criar soluções úteis via Vibe Coding. Mesmo com a limitação pontual do erro 503 (fora do meu controle), o app entrega valor real ao usuário:
- ✅ Controle de gastos por conversa
- ✅ Menu rápido por categorias
- ✅ Metas financeiras personalizadas
- ✅ Painel dinâmico com gráficos
- ✅ Agente amigável que incentiva e educa

---

## 📂 Entrega

Este projeto foi desenvolvido como parte do desafio do **curso de IA da DIO**.

- **Ferramenta utilizada:** Google AI Studio com agente Antigravity
- **Abordagem:** Vibe Coding (100% via prompts, sem código manual)
