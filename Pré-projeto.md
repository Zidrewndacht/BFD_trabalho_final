
# Pré-projeto — Definição do Entregável

- **Prazo:** Previsto 14/07/2026  
- **Formato:** Documento Markdown no repositório do projeto (`docs/pre_projeto.md`) ou PDF de 2–4 páginas  
  - Alunos devem portanto escolher um mantenedor que enviará o link do repositório do projeto nesta etapa.
  - O professor deverá ter acesso ao repositório durante o desenvolvimento.
 - **Objetivo:** Convencer o professor de que a ideia é viável, útil e do tamanho certo.

---

## Estrutura Obrigatória

### 1. Identificação da Equipe
- Nome do projeto (pode ser provisório)
- Nome e GitHub de cada membro
- Divisão preliminar de responsabilidades (quem cuida do quê?)

### 2. Elevator Pitch (máx. 3 frases)
> *"Para [público-alvo] que [problema], [nome do projeto] é uma aplicação web que [solução principal]. Diferente de [alternativa manual/existente], nós [diferencial]."*

### 3. Público-Alvo e Contexto
- Quem vai usar? (Ex: "bibliotecário de escola", "organizador de eventos da faculdade", "cozinheiro caseiro")
- Em que situação? (Ex: "no computador da biblioteca", "no celular durante feira")
- Por que isso é melhor que planilha/papel/WhatsApp?

### 4. Funcionalidades principais (máximo 5)
Liste o que a aplicação **deve fazer** para ser considerada terminada.  
Use o formato: *"Como [usuário], quero [ação] para [resultado]"*.

Exemplo adequado:
1. Cadastrar livros com título, autor, ano e gênero
2. Buscar livros por título ou autor
3. Marcar livro como emprestado para um aluno
4. Ver histórico de empréstimos de um livro
5. Exportar lista de livros atrasados como HTML

### 5. Escopo Negativo — O que NÃO faremos
Liste explicitamente o que parece esperado em uma aplicação com a sua finalidade, mas está **fora** do projeto.  
Exemplos:
- "Não teremos pagamentos online"
- "Não será um app mobile nativo (apenas web responsiva)"
- "Não usaremos IA para recomendação automática"
- "Não teremos notificações por e-mail/SMS"

### 6. Modelo de Dados Preliminar
Liste as **entidades** (tabelas) e seus **relacionamentos** em português simples.  
Não precisa ser diagrama formal. Exemplo:

```
LIVRO (id, titulo, autor, ano, genero, disponivel)
EMPRESTIMO (id, livro_id, aluno_nome, data_emprestimo, data_devolucao)
Relacionamento: um Livro tem muitos Emprestimos
```

### 8. Wireframes (obrigatório)
Anexe **fotos de rabiscos no papel** ou screenshots de ferramentas simples (Excalidraw, draw.io, Figma, Paint).  
Deve haver:
- Ao menos uma tela para **computador**
- Ao menos uma tela para **celular**

### 9. Stack Confirmado
Confirme que usarão:
- [ ] Flask + Jinja2
- [ ] SQLite/PostgreSQL/MariaDB
- [ ] HTML + CSS Grid + JS Vanilla
- [ ] GitHub com PRs

Justifique em uma frase cada biblioteca adicional (não built-in) que planejam utilizar.

### 10. Autoavaliação de Riscos
Responda honestamente:
1. Qual é a parte que vocês **mais temem** implementar?
2. O que acontece se um membro da equipe sumir 1 semana antes da entrega?
3. Qual é o "caminho feliz" mínimo que entrega valor mesmo se tudo mais falhar?