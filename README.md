# 🧠 Recruiter Specialist AI Agent (Langflow + OpenAI)

Este projeto é um agente de Inteligência Artificial construído com a ferramenta **Langflow** e integrado à API da **OpenAI**, utilizando o modelo `gpt-4o-mini`. Seu objetivo é atuar como um **Recruiter Specialist**, ajudando a adaptar currículos de candidatos a vagas específicas, de forma personalizada e automatizada.

---

## ⚙️ Como Funciona

O fluxo é composto por 5 principais componentes conectados no Langflow:

1. **🔗 URL**  
   Permite capturar os dados de perfil de um candidato a partir de um link da DIO (https://www.dio.me/users/...).

2. **📄 Prompt**  
   Um template dinâmico recebe dois inputs principais:
   - `{CANDIDATO}` → Dados do perfil do usuário extraídos da URL
   - `{VAGA}` → Descrição da vaga desejada

3. **🤖 Agent**  
   - Provider: `OpenAI`  
   - Model Name: `gpt-4o-mini`  
   - API Key: (é necessário inserir a sua chave da OpenAI)  
   - Instruções: O agente é instruído a analisar os dados do candidato e da vaga, e gerar uma resposta formatada com:
     - Resumo profissional
     - Principais habilidades
     - Conquistas ou certificações
     - Artigos publicados
     - Análise de aderência à vaga

4. **🧠 Chat Input**  
   Campo de entrada manual para personalizar ou complementar os dados.

5. **💬 Chat Output**  
   Exibe a resposta gerada pelo agente em linguagem natural.

---

## 📝 Exemplo de Aplicação

Este agente pode ser utilizado por profissionais de RH, desenvolvedores de sistemas de recrutamento, ou candidatos que desejam personalizar seu currículo para diferentes vagas de forma automatizada.

---

## 📌 Requisitos

- Conta na [OpenAI](https://platform.openai.com/)
- Chave da API inserida no bloco "Agent"
- Conta gratuita no [Langflow](https://github.com/logspace-ai/langflow)
- Link de perfil válido da DIO para entrada de dados

---

## 💡 Observações

- O modelo `gpt-4o-mini` é leve e pode ser utilizado com menor custo, mas **ainda requer uma chave de API válida**, mesmo sendo gratuito em ambientes como o ChatGPT web.
- Este projeto não armazena dados, funcionando inteiramente em tempo real com base na entrada.

---

## 🖼️ Visual do Fluxo

![Fluxo do Agente no Langflow](./screenshot.png)

> Substitua o caminho da imagem (`./screenshot.png`) pela localização correta caso vá hospedar este repositório no GitHub.

---

## 🚀 Próximos Passos

- Adicionar validação automática dos dados do candidato
- Integrar com serviços de envio de e-mail para entrega do currículo personalizado
- Permitir múltiplas vagas e rankings de aderência

---

Desenvolvido usando Langflow + OpenAI
