### dio-lab-vibe-coding-ATS-friendly-curriculum-generator
Processo de criação de um Gerador de Currículos ATS Friendly por Vibe Coding no Lovable.
---
<img width="1366" height="638" alt="image" src="https://github.com/user-attachments/assets/faa34ab8-edf7-4ae3-820f-3d6c123dc897" />

# Problema que o Matchpoint resolve

O Matchpoint resolve o problema da **dificuldade de encontrar oportunidades de emprego compatíveis com o próprio perfil profissional e adaptar o currículo para cada candidatura de maneira estratégica e eficiente.**

Atualmente, candidatos enfrentam três problemas principais:

### 1. Dificuldade de identificar oportunidades compatíveis
Encontrar vagas adequadas às próprias qualificações exige tempo e análise manual de inúmeros requisitos.

### 2. Currículos pouco direcionados
Muitos candidatos utilizam o mesmo currículo para diferentes oportunidades, sem destacar as experiências e competências mais relevantes para cada posição.

### 3. Dificuldade de otimização para ATS
Candidatos nem sempre sabem identificar e incorporar palavras-chave relevantes ou estruturar seus currículos para facilitar a leitura pelos sistemas automatizados de recrutamento.

## Solução proposta

O Matchpoint utiliza inteligência artificial para conectar as qualificações reais do candidato às exigências das oportunidades profissionais, identificar compatibilidades e lacunas e gerar currículos personalizados e otimizados para ATS.

## Proposta de valor

**O Matchpoint transforma uma busca de emprego genérica em um processo de candidatura direcionado, inteligente e personalizado.**

Reduzir o tempo e o esforço necessários para encontrar vagas compatíveis e preparar candidaturas relevantes, aumentando a capacidade do candidato de apresentar suas qualificações de maneira estratégica, sem comprometer a veracidade de sua trajetória profissional.

---
# Prompt único para o Lovable
```markdown
## Criação de SaaS: Matchpoint | Matchmaking de Vagas e Otimização de Currículos ATS

Atue como um desenvolvedor full-stack sênior, especialista em UX/UI Design e arquitetura de produtos SaaS.

Crie do zero uma aplicação web chamada **Matchpoint**, uma plataforma inteligente de matchmaking entre candidatos e oportunidades de emprego, com geração de currículos personalizados e otimizados para sistemas ATS (Applicant Tracking Systems).

O objetivo é entregar um MVP funcional, visualmente sofisticado e com arquitetura simples, priorizando as funcionalidades essenciais do produto.

**IMPORTANTE:** Estou utilizando o plano gratuito do Lovable e tenho um orçamento limitado de créditos. Portanto, implemente tudo em uma única execução, tome decisões de produto autonomamente e evite perguntas desnecessárias, funcionalidades secundárias e alterações arquiteturais complexas.

---

## 1. CONCEITO DO PRODUTO

O Matchpoint é uma plataforma que ajuda candidatos a encontrar oportunidades profissionais compatíveis com seu perfil e adaptar seus currículos para cada candidatura.

O usuário deverá conseguir:

1. Criar e manter seu perfil profissional.
2. Inserir ou importar seu currículo atual.
3. Cadastrar oportunidades de emprego.
4. Analisar a compatibilidade entre seu perfil e os requisitos de cada vaga.
5. Identificar habilidades correspondentes e lacunas de qualificação.
6. Gerar versões personalizadas de seu currículo para cada oportunidade.
7. Editar, salvar e exportar cada versão do currículo.

O produto deve transmitir a sensação de uma ferramenta premium de gestão de carreira, e não de um portal genérico de empregos.

Nome provisório: **Matchpoint**.

## 2. IDENTIDADE VISUAL E DESIGN SYSTEM

Utilize obrigatoriamente **shadcn/ui** como design system principal.

Tecnologias:
- React
- TypeScript
- Tailwind CSS
- shadcn/ui
- Lucide Icons

### Paleta de cores

Utilize a seguinte identidade visual:

- Azul-marinho principal: #172B45
- Caramelo: #B98255
- Marfim: #F5F2EC
- Branco: #FFFFFF
- Cinza-ardósia: #667085
- Cinza para bordas: #E5E1DA
- Verde para indicadores positivos: #36856A
- Âmbar para alertas: #D69B48

Diretrizes de aplicação:
- Azul-marinho para navegação, títulos importantes e ações primárias.
- Caramelo para destaques, elementos secundários e detalhes visuais.
- Marfim como cor de fundo predominante.
- Branco para cartões e superfícies de conteúdo.
- Cinza-ardósia para textos secundários.

### Direção estética

Desenvolva uma interface sofisticada, profissional, elegante e acolhedora.

Referências conceituais: plataformas SaaS premium, interfaces editoriais contemporâneas e produtos digitais de produtividade.

Utilize:
- Hierarquia visual clara.
- Espaçamentos consistentes.
- Bordas discretas.
- Sombras sutis.
- Cantos arredondados entre 8px e 12px.
- Tipografia elegante e legível.
- Microinterações discretas.
- Excelente responsividade.

Utilize Inter para os textos da interface e DM Serif Display para títulos editoriais selecionados.

Evite:
- Gradientes excessivos.
- Cores vibrantes.
- Aparência genérica de ferramentas de IA.
- Elementos decorativos desnecessários.
- Excesso de arredondamentos.
- Interfaces visualmente carregadas.

## 3. ESTRUTURA DA APLICAÇÃO

Crie as seguintes páginas:

### A. Dashboard

O dashboard será o espaço principal de trabalho do usuário.

Inclua:

- Mensagem de boas-vindas.
- Indicador de preenchimento do perfil profissional.
- Quantidade de vagas salvas.
- Quantidade de currículos personalizados.
- Compatibilidade média das vagas analisadas.
- Vagas adicionadas recentemente.
- Currículos editados recentemente.
- Botão principal: "Encontrar oportunidades".
- Botão secundário: "Atualizar meu currículo".

Crie também um estado inicial para usuários novos, incentivando o preenchimento do perfil profissional.

### B. Meu Perfil

Crie um editor de perfil profissional dividido nas seguintes seções:

**Informações pessoais**
- Nome completo.
- Título profissional.
- E-mail.
- Telefone.
- Cidade e país.
- LinkedIn.
- Portfólio.

**Resumo profissional**
- Apresentação profissional.
- Objetivos de carreira.

**Experiência profissional**

Permita adicionar, editar e excluir experiências.

Campos:
- Cargo.
- Empresa.
- Data de início.
- Data de término.
- Responsabilidades.
- Principais realizações.

**Formação acadêmica**
- Instituição.
- Curso.
- Grau de formação.
- Ano de conclusão.

**Competências**
- Habilidades técnicas.
- Habilidades interpessoais.
- Ferramentas e softwares.

**Idiomas**
- Idioma.
- Nível de proficiência.

Permita que o usuário importe seu currículo existente ou insira as informações manualmente.

### C. Encontrar Vagas

Crie uma área dedicada ao matchmaking de oportunidades.

Nesta primeira versão, o usuário deverá cadastrar vagas manualmente, utilizando:

- Descrição completa da vaga, por texto.
- Nome da empresa.
- Título do cargo.
- Localização, quando disponível.
- URL original da oportunidade, opcional.

Não implemente scraping de sites externos ou dependência de APIs pagas de empregos.

Após o cadastro, compare a descrição da vaga com o perfil profissional do usuário.

Cada oportunidade deverá aparecer em um cartão contendo:

- Nome do cargo.
- Empresa.
- Localização.
- Percentual de compatibilidade.
- Principais competências correspondentes.
- Competências ausentes ou pouco evidenciadas.
- Breve explicação sobre a compatibilidade.

Inclua filtros por:
- Percentual de compatibilidade.
- Empresa.
- Cargo.

Utilize as seguintes classificações:

- 85% a 100%: Excelente compatibilidade.
- 70% a 84%: Alta compatibilidade.
- 50% a 69%: Compatibilidade parcial.
- Abaixo de 50%: Baixa compatibilidade.

A pontuação deverá ser baseada em critérios reais de comparação entre o perfil e os requisitos da vaga. Nunca utilize pontuações aleatórias ou fictícias.

### D. Detalhes da Vaga

Ao selecionar uma oportunidade, apresente uma análise detalhada.

**Compatibilidade geral**

Exiba o percentual de compatibilidade em destaque, acompanhado de um indicador visual de progresso.

**Comparação de competências**

Organize as competências em três grupos:

- Competências correspondentes.
- Competências ausentes.
- Competências adicionais do candidato.

**Compatibilidade de experiência**

Explique como as experiências profissionais anteriores se relacionam com os requisitos da oportunidade.

**Compatibilidade acadêmica**

Compare a formação do candidato com os requisitos educacionais da vaga.

**Recomendações**

Apresente sugestões práticas para melhorar a candidatura, sem sugerir que o candidato invente qualificações.

Inclua um botão de destaque:

"Criar currículo personalizado"

### E. Criador de Currículos ATS

Esta é a funcionalidade central do Matchpoint e deve receber prioridade na implementação.

O sistema deverá gerar um currículo personalizado utilizando três fontes:

1. Perfil profissional original do usuário.
2. Descrição da vaga selecionada.
3. Análise de compatibilidade realizada anteriormente.

O currículo gerado deverá:

- Incorporar naturalmente palavras-chave relevantes da descrição da vaga.
- Priorizar experiências profissionais relevantes.
- Adaptar o resumo profissional ao cargo pretendido.
- Destacar competências relacionadas à oportunidade.
- Utilizar títulos de seção convencionais.
- Apresentar estrutura linear e simples.
- Evitar tabelas, colunas, gráficos, ícones e elementos que dificultem a leitura por sistemas ATS.
- Utilizar tipografia legível.
- Manter uma apresentação profissional.

**REGRAS FUNDAMENTAIS DE PRECISÃO:**

Nunca invente:
- Experiências profissionais.
- Habilidades.
- Certificações.
- Diplomas.
- Resultados profissionais.
- Datas.
- Empresas.
- Responsabilidades que não foram informadas pelo usuário.

Nunca exagere as qualificações do candidato.

Se a vaga exigir uma competência que o usuário não possui, não a inclua como se fosse uma habilidade dele.

O sistema deve reorganizar, reescrever e enfatizar informações verdadeiras, preservando seu significado original.

### Interface do editor de currículos

Crie uma interface dividida em duas áreas:

**Área de edição**
- Editor de texto.
- Seções editáveis.
- Possibilidade de editar o resumo profissional.
- Possibilidade de editar experiências.
- Possibilidade de editar competências.
- Botão para regenerar uma seção específica.

**Área de visualização**
- Pré-visualização do currículo.
- Formatação simples e profissional.
- Visualização semelhante ao documento exportado.

Inclua as seguintes ações:

- Editar currículo.
- Salvar versão.
- Duplicar versão.
- Regenerar seção.
- Exportar para PDF.
- Exportar para DOCX, caso seja possível implementar com as bibliotecas disponíveis.

Cada currículo deverá estar associado à oportunidade para a qual foi criado.

Apresente um aviso discreto informando que a otimização ATS melhora a legibilidade e a interpretação do documento, mas não garante aprovação ou contratação.

### F. Meus Currículos

Crie uma biblioteca de currículos personalizados.

Cada item deverá apresentar:

- Nome do currículo.
- Cargo pretendido.
- Empresa.
- Data de criação.
- Última atualização.
- Percentual de compatibilidade.

Permita:
- Abrir e editar.
- Duplicar.
- Renomear.
- Excluir.
- Exportar.

## 4. FUNCIONALIDADES DE INTELIGÊNCIA ARTIFICIAL

Utilize o Lovable AI, caso esteja disponível no ambiente, para implementar:

1. Extração de informações de currículos.
2. Interpretação de descrições de vagas.
3. Cálculo de compatibilidade profissional.
4. Identificação de lacunas de competências.
5. Geração de currículos personalizados.
6. Sugestões de melhorias para candidaturas.

Crie instruções específicas para cada operação.

Sempre que possível, solicite respostas estruturadas em JSON para facilitar a integração com a interface.

A IA deverá considerar o contexto completo do candidato e da oportunidade.

Não simule funcionalidades de IA com resultados aleatórios ou textos estáticos apresentados como análises reais.

Se alguma funcionalidade depender de ativação ou configuração adicional, deixe essa dependência explícita e não apresente uma operação simulada como se tivesse sido concluída.

Não exija APIs pagas ou chaves externas fornecidas manualmente caso o Lovable AI consiga executar a funcionalidade.

## 5. BANCO DE DADOS E PERSISTÊNCIA

Utilize os recursos do Lovable Cloud quando disponíveis.

Para esta primeira versão:

- Não implemente autenticação.
- Não implemente sistemas complexos de permissões.
- Persista os dados do perfil profissional.
- Persista as oportunidades cadastradas.
- Persista os currículos gerados.
- Utilize uma estrutura de dados simples e organizada.
- Caso a configuração de backend não esteja disponível, utilize persistência local como alternativa.

Os dados devem continuar disponíveis após atualizar a página.

Organize a estrutura para permitir a implementação futura de autenticação e múltiplos usuários sem precisar reconstruir toda a aplicação.

## 6. EXPERIÊNCIA DO USUÁRIO

O fluxo principal deverá ser:

1. O usuário acessa a aplicação.
2. Completa seu perfil profissional ou importa seu currículo.
3. Cadastra uma oportunidade de emprego.
4. O sistema analisa a compatibilidade.
5. O usuário visualiza os resultados.
6. Seleciona a opção de criar um currículo personalizado.
7. Edita e salva o documento.
8. Exporta a versão final.

O fluxo deve ser intuitivo, rápido e sem etapas desnecessárias.

Implemente:
- Estados de carregamento.
- Mensagens de sucesso.
- Mensagens de erro.
- Validação de formulários.
- Confirmações antes de exclusões.
- Estados vazios com orientações.
- Feedback visual para todas as ações.

Todos os botões e elementos interativos devem funcionar. Não crie botões meramente decorativos.

## 7. NAVEGAÇÃO

Crie uma sidebar lateral para desktop contendo:

- Dashboard.
- Meu Perfil.
- Encontrar Vagas.
- Meus Currículos.
- Configurações.

Adicione o logotipo tipográfico Matchpoint no topo da sidebar.

Em dispositivos móveis, utilize navegação compacta e responsiva.

## 8. REQUISITOS FINAIS

Entregue um MVP funcional, coeso e visualmente refinado.

Priorize nesta ordem:

1. Design profissional e consistente.
2. Editor de perfil profissional.
3. Cadastro de oportunidades.
4. Análise de compatibilidade.
5. Geração e edição de currículos ATS.
6. Persistência dos dados.
7. Exportação dos documentos.

Não implemente nesta versão:

- Rede social.
- Chat.
- Sistema de assinaturas.
- Pagamentos.
- Analytics avançado.
- Integrações com plataformas externas de empregos.
- Contas para recrutadores.
- Questionários extensos de onboarding.

Não adicione funcionalidades fora do escopo definido.

**INSTRUÇÃO FINAL:**

Implemente diretamente a aplicação completa. Não entregue apenas uma landing page, protótipo visual ou dashboard estático.

O resultado deverá ser uma aplicação utilizável, com navegação funcional, formulários operacionais, persistência de dados e fluxo completo de matchmaking e personalização de currículos.

Tome decisões de implementação autonomamente, priorizando simplicidade, qualidade visual e funcionamento real das funcionalidades essenciais.
```
>Obs.: Como estava com poucos créditos para terminar a tempo fazendo correções, me esforcei para que este primeiro megaprompt para que fosse o mais acertivo possível, e felizmente atingi o meu objetivo, porque os créditos acabaram.
---
### Importe seu currículo
><img width="1366" height="640" alt="image" src="https://github.com/user-attachments/assets/f95e7373-4edc-4874-8cab-564ef3eed05d" />

### Veja o Dashboard com base em seu perfil
<img width="1366" height="633" alt="image" src="https://github.com/user-attachments/assets/d1de503f-f2de-4fed-83d0-ff8618b3aac0" />

### Inclua a vaga de emprego de seu interesse 
<img width="1366" height="637" alt="image" src="https://github.com/user-attachments/assets/2048df40-7968-427a-8859-25262c0584e3" />

### Analise a sua compatibilidade com a vaga
<img width="1366" height="635" alt="image" src="https://github.com/user-attachments/assets/f433055f-8e2f-48c4-ac8b-81311fb667fa" />

### Gere um currículo com base na vaga almejada
<img width="1366" height="638" alt="image" src="https://github.com/user-attachments/assets/e8cf804f-f7bc-4751-b753-1158681d7427" />


# Como funciona a análise do Matchpoint

O Matchpoint utiliza inteligência artificial para comparar o perfil profissional do candidato com os requisitos de uma oportunidade de emprego e gerar uma versão personalizada do currículo, otimizada para sistemas ATS (Applicant Tracking Systems).

O processo é dividido em seis etapas:

### 1. Interpretação da vaga
O usuário cola a descrição da oportunidade. A IA analisa o conteúdo e extrai informações estruturadas, identificando:
- Requisitos obrigatórios e desejáveis.
- Competências técnicas e comportamentais.
- Experiência profissional exigida.
- Formação acadêmica.
- Ferramentas e tecnologias.
- Palavras-chave relevantes para ATS.
- Responsabilidades e senioridade.

### 2. Análise do perfil profissional
O sistema compara os requisitos identificados com o currículo-mestre do usuário, verificando experiências, formação, competências, idiomas e qualificações.

### 3. Cálculo de compatibilidade (Match Score)
O sistema calcula um percentual de compatibilidade considerando cinco dimensões:
- Competências técnicas.
- Experiência profissional.
- Formação acadêmica.
- Ferramentas e tecnologias.
- Idiomas e requisitos adicionais.

O resultado apresenta os pontos fortes, requisitos parcialmente atendidos e competências não identificadas no perfil.

### 4. Identificação de experiências relevantes
A IA seleciona as experiências, realizações e competências mais relevantes para a oportunidade, priorizando informações que demonstrem a adequação do candidato à vaga.

### 5. Geração do currículo personalizado
Com base na análise, a IA cria uma nova versão do currículo:
- Adapta o resumo profissional.
- Reorganiza as experiências por relevância.
- Melhora a descrição de responsabilidades e realizações.
- Destaca competências compatíveis.
- Incorpora naturalmente palavras-chave da vaga.
- Utiliza estrutura simples e legível por sistemas ATS.

**Regra fundamental:** nenhuma experiência, competência, formação, certificação ou realização pode ser inventada. A IA deve trabalhar exclusivamente com informações fornecidas ou confirmadas pelo candidato.

### 6. Validação e exportação
Antes da entrega, o currículo passa por uma verificação de:
- Estrutura e formatação ATS-friendly.
- Presença de palavras-chave relevantes.
- Correspondência com os requisitos da vaga.
- Fidelidade às informações do candidato.
- Integridade dos dados pessoais e profissionais.

Após a validação, o usuário pode editar, salvar e exportar o currículo personalizado em PDF ou DOCX.

---

## Fluxo resumido

```text
Descrição da vaga
       ↓
Interpretação dos requisitos
       ↓
Comparação com o perfil profissional
       ↓
Cálculo do Match Score
       ↓
Identificação de experiências relevantes
       ↓
Geração do currículo personalizado
       ↓
Validação ATS e de fidelidade
       ↓
Edição e exportação
```

## Princípio central

O Matchpoint mantém um **currículo-mestre** como fonte de verdade e gera versões independentes e personalizadas para cada oportunidade.
Dessa forma, o usuário pode adaptar suas candidaturas sem perder o histórico profissional original ou comprometer a veracidade das informações.

---
# Link para o Matchpoint

>https://matchpoint-dot.lovable.app/

