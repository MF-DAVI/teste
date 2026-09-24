# 📋 Projeto de APS — PlantTinder

## Levantamento e Priorização de Requisitos

**Curso:** Engenharia de Software  
**Disciplina:** Análise e Projeto de Sistemas / Engenharia de Software  
**Instituição:** UDF Centro Universitário  
**Etapa:** Levantamento de Requisitos e Fichas de Elicitação  
**Técnica de Priorização:** MoSCoW  
**Data:** 24/09/2026  
**Turma:** D2 | **Versão:** 1.0  
**Link do Board/Template:** https://miro.com/app/board/uXjVHo3jFqo=/  

---

# 👥 1. Identificação do Grupo

| Integrante | Nome | Perfil / Repositório |
|---|---|---|
| 1 | João Pedro Alves De Sousa | [jpedro-swe](https://github.com/jpedro-swe) |
| 2 | Hélter Brandão De Oliveira | [brandao395](https://github.com/brandao395) |
| 3 | Davi Gonçalves Castro | [MF-DAVI](https://github.com/MF-DAVI) |
| 4 | Jorge Luis Soares do Santos | [7deo](https://github.com/7deo) |

---

# 2. Identificação do Projeto

**Nome do projeto:**  
> Rede de Apoio para Adoção de Plantas (PlantTinder)

**Descrição resumida do projeto:**  
> O projeto consiste no desenvolvimento de uma plataforma digital focada em conectar pessoas interessadas em adotar plantas com doadores. O objetivo principal é facilitar a adoção responsável por meio do matching de perfis, gerenciamento de anúncios e comunicação direta entre os usuários.

---

# 3. Problema Identificado

## 3.1 Qual problema será resolvido?

> A dificuldade de encontrar destinos adequados para plantas que não podem mais ser cuidadas pelos seus atuais donos, bem como a dificuldade de entusiastas de plantas encontrarem espécies específicas para adoção de forma confiável e centralizada.

## 3.2 Quem é afetado pelo problema?

> Entusiastas de plantas, jardineiros, pessoas que precisam doar suas plantas por falta de espaço ou tempo, e interessados em práticas de adoção sustentável.

## 3.3 Como o problema é resolvido atualmente?

> Atualmente, as pessoas dependem de redes sociais genéricas, grupos de vizinhança ou doações boca a boca, o que dificulta o encontro entre doadores e pessoas com o perfil adequado para cuidar da planta específica, além de carecer de histórico ou garantias de cuidado.

## 3.4 Principais dificuldades encontradas

1. Falta de uma plataforma centralizada e confiável para doação de plantas.
2. Dificuldade em encontrar pessoas com o conhecimento adequado para cuidar de espécies específicas.
3. Comunicação fragmentada e desorganizada entre doadores e adotantes.

---

# 🎯 4. Objetivo do Projeto

**Objetivo:**

> Nosso projeto pretende criar uma plataforma centralizada e segura para doadores e adotantes de plantas, contribuindo para a adoção responsável e sustentável, facilitando o encontro de perfis compatíveis com as necessidades de cada espécie.

---

# 👤 5. Stakeholders

| ID | Stakeholder | Papel | Necessidade/Interesse | Influência |
|---|---|---|---|---|
| ST01 | Doadores de Plantas | Usuário | Encontrar lares adequados para suas plantas de forma fácil e segura. | Alta |
| ST02 | Adotantes de Plantas | Usuário | Encontrar plantas disponíveis para adoção que se adequem ao seu perfil e localização. | Alta |
| ST03 | Administradores do Sistema | Manutenção/Suporte | Garantir o funcionamento, segurança e integridade da plataforma. | Média |

## Stakeholder principal

**Stakeholder:**
> Doadores e Adotantes de Plantas (Usuários Finais)

**Por que ele foi considerado o principal stakeholder?**
> Porque o sucesso e a utilidade da plataforma dependem inteiramente do engajamento e da interação entre esses dois grupos. Sem eles, o sistema não tem propósito.

---

# 🗣️ 6. Levantamento de Informações

| Pergunta | Resposta |
|---|---|
| O que o usuário precisa fazer? | Cadastrar-se, anunciar plantas, buscar plantas, comunicar-se e avaliar a experiência. |
| Qual problema enfrenta atualmente? | Dificuldade em encontrar e doar plantas de forma estruturada e confiável. |
| Quais informações precisa consultar? | Espécies disponíveis, detalhes e cuidados da planta, localização do doador e avaliações. |
| Quais informações precisa cadastrar ou alterar? | Dados pessoais, preferências de plantas, fotos e detalhes dos anúncios de doação. |
| Quais tarefas são repetitivas? | Responder a perguntas básicas sobre a planta anunciada (mitigado pelo preenchimento de detalhes no anúncio). |
| Quais tarefas consomem mais tempo? | Filtrar e encontrar a planta ideal ou o adotante ideal. |
| Quais erros acontecem atualmente? | Doações para pessoas sem perfil para cuidar da espécie, falta de informações sobre os cuidados necessários. |
| Precisa receber notificações? | Sim, para novos pedidos de adoção e novas mensagens recebidas. |
| Precisa gerar documentos ou relatórios? | Não, o sistema é focado em matchmaking e comunicação. |
| Existem informações que precisam ser protegidas? | Sim, dados pessoais dos usuários, como e-mail, telefone e localização exata (proteção LGPD). |
| O sistema precisará se comunicar com outros sistemas? | Pode necessitar comunicação com APIs de mapas/geolocalização. |
| Existem regras obrigatórias que precisam ser respeitadas? | Lei Geral de Proteção de Dados (LGPD). |

---

# 💡 7. Necessidades Identificadas

| ID | Stakeholder | Necessidade Identificada | Problema Relacionado |
|---|---|---|---|
| N01 | Todos os usuários | Criar uma conta para acessar a plataforma. | Falta de ambiente seguro e rastreável. |
| N02 | Doador | Publicar informações detalhadas sobre a planta disponível. | Falta de clareza sobre os cuidados que a planta exige. |
| N03 | Adotante | Pesquisar plantas por características específicas (ex: tamanho, espécie, local). | Dificuldade em encontrar plantas adequadas ao seu perfil e região. |
| N04 | Adotante | Demonstrar interesse formal em uma planta. | Falta de um processo claro de adoção. |
| N05 | Todos os usuários | Trocar mensagens para combinar a entrega. | Comunicação desorganizada em redes sociais diversas. |
| N06 | Todos os usuários | Segurança dos dados pessoais informados. | Exposição indevida de dados na internet. |

---

# ⚙️ 8. Requisitos Funcionais

| ID | Requisito Funcional | Stakeholder/Fonte | Necessidade | Prioridade |
|---|---|---|---|---|
| RF01 | O sistema deve permitir que novos usuários se cadastrem na plataforma informando seus dados pessoais e preferências de plantas. | Todos os usuários | N01 | Alta |
| RF02 | O sistema deve permitir que usuários anunciem plantas disponíveis para adoção com detalhes sobre a espécie e cuidados necessários. | Doadores | N02 | Alta |
| RF03 | O sistema deve permitir que usuários busquem plantas disponíveis para adoção usando filtros como espécie, tamanho e localização. | Adotantes | N03 | Alta |
| RF04 | O sistema deve permitir que interessados em adotar enviem pedidos formais ao doador da planta. | Adotantes | N04 | Alta |
| RF05 | O sistema deve permitir troca de mensagens entre doador e adotante para discussão dos detalhes da entrega. | Todos os usuários | N05 | Alta |
| RF06 | O sistema deve permitir que usuários avaliem doadores e adotantes após a conclusão da adoção. | Todos os usuários | - | Média |
| RF07 | O sistema deve permitir que usuários atualizem seus dados pessoais, preferências e foto de perfil. | Todos os usuários | - | Média |

---

# ⭐ 9. Requisitos de Qualidade (Não Funcionais)

| ID | Característica de Qualidade | Requisito | Como será verificado? |
|---|---|---|---|
| RNF01 | Segurança | O sistema deve controlar o acesso às funcionalidades conforme o perfil do usuário e proteger dados pessoais conforme LGPD. Senhas criptografadas. | Testes de penetração, verificação de criptografia no banco e auditoria de acesso a dados. |
| RNF02 | Usabilidade | A interface deve apresentar informações claras, ser intuitiva e responsiva para dispositivos móveis. Mensagens de erro claras. | Testes de usabilidade com usuários e validação de responsividade em diferentes telas. |
| RNF03 | Desempenho | Buscas de plantas devem retornar resultados em até 2 segundos e carregamento de fotos em até 3 segundos. | Testes de carga e monitoramento de tempo de resposta do servidor. |
| RNF04 | Disponibilidade | O sistema deve ter disponibilidade mínima de 99% do tempo, operando 24/7. | Monitoramento contínuo de uptime do servidor. |
| RNF05 | Integridade | O sistema deve preservar a consistência, impedindo anúncio sem dados essenciais e exclusão de plantas com pedidos pendentes. | Testes unitários e de integração validando as regras de banco de dados e backend. |
| RNF06 | Escalabilidade | O sistema deve suportar no mínimo 10.000 usuários simultâneos sem degradação de desempenho. | Testes de stress simulando múltiplos acessos simultâneos. |

---

# 🚧 10. Restrições

| ID | Restrição | Categoria | Justificativa/Fonte |
|---|---|---|---|
| RES01 | Adequação à LGPD | Legislação | Obrigatório para tratamento de dados pessoais no Brasil. |
| RES02 | Escopo exclusivamente gratuito | Negócio | A plataforma não suportará vendas ou transações financeiras, focando apenas em doação/adoção. |
| RES03 | Prazos acadêmicos | Prazo | O projeto deve ser concluído dentro do cronograma da disciplina de Engenharia de Software. |

---

# 📜 11. Regras de Negócio

| ID | Regra de Negócio | Fonte |
|---|---|---|
| RN01 | Usuários devem estar autenticados para acessar funções sensíveis, como enviar pedidos ou mensagens. | RNF01 (Segurança) |
| RN02 | Uma planta não pode ser excluída do sistema enquanto houver pedidos de adoção pendentes associados a ela. | RNF05 (Integridade) |
| RN03 | Apenas o usuário proprietário (doador) pode aceitar ou rejeitar um pedido de adoção para sua planta. | RF04 (Pedidos) |

---

# 🔗 12. Rastreabilidade Inicial

| Necessidade | Stakeholder | Requisito(s) relacionado(s) |
|---|---|---|
| N01 | Todos os usuários | RF01, RNF01 |
| N02 | Doador | RF02, RNF05 |
| N03 | Adotante | RF03, RNF03 |
| N04 | Adotante | RF04, RNF05 |
| N05 | Todos os usuários | RF05, RNF03 |
| N06 | Todos os usuários | RNF01 |

---

# 🏷️ 13. Priorização dos Requisitos — Técnica MoSCoW

## Matriz de Priorização

| ID | Requisito | MoSCoW | Justificativa |
|---|---|:---:|---|
| RF01 | Cadastrar usuário | M | Sem cadastro, não há controle de usuários ou segurança. |
| RF02 | Anunciar planta | M | Funcionalidade core do sistema (oferta). |
| RF03 | Buscar e filtrar | M | Funcionalidade core do sistema (demanda). |
| RF04 | Enviar pedido | M | Mecanismo principal de conexão entre as partes. |
| RF05 | Comunicação | M | Essencial para viabilizar a entrega da planta. |
| RF06 | Avaliar e comentar | C | Bom para gerar confiança, mas o sistema funciona sem isso na V1. |
| RF07 | Gerenciar perfil | S | Importante para manter dados atualizados, mas pode ser feito em uma segunda iteração se necessário. |
| RNF01 | Segurança | M | Proteção de dados é requisito legal (LGPD). |
| RNF02 | Usabilidade | M | Garante que o público-alvo conseguirá usar a ferramenta. |
| RNF03 | Desempenho | S | Tempos de resposta otimizados são importantes, mas uma leve lentidão na V1 não impede o uso. |
| RNF04 | Disponibilidade | M | O sistema precisa estar no ar para cumprir seu papel. |
| RNF05 | Integridade | M | Evita corrupção de dados e falhas nas transações de adoção. |
| RNF06 | Escalabilidade | C | Otimização para grandes volumes pode ser implementada conforme o crescimento real. |

---

# 🚀 14. Requisitos da Primeira Versão (MVP)

| Ordem | ID | Requisito | Por que deve estar na primeira versão? |
|:---:|---|---|---|
| 1 | RF01 | Cadastrar usuário | Garante a base de usuários autenticados, essencial para rastreabilidade e segurança. |
| 2 | RF02 | Anunciar planta para adoção | É o que alimenta o sistema com o "produto" (plantas), sem isso não há o que adotar. |
| 3 | RF03 | Buscar e filtrar plantas | Permite que os interessados encontrem as plantas anunciadas. |
| 4 | RF04 | Enviar pedido de adoção | Formaliza o interesse e inicia o processo de adoção. |
| 5 | RF05 | Comunicação entre usuários | Permite o alinhamento logístico (entrega/retirada) para concluir a adoção. |

---

# ⏭️ 15. Requisitos para Versões Futuras

| ID | Requisito | Motivo para adiar | Impacto |
|---|---|---|---|
| RF06 | Avaliar e comentar | Requisito "Could Have". O fluxo principal de adoção funciona sem o sistema de reputação inicialmente. | Menor confiança inicial entre desconhecidos. |
| RNF06 | Escalabilidade (10.000 usuários) | Requisito "Could Have". A base de usuários inicial será pequena, permitindo otimizar a infraestrutura depois. | Possível lentidão se houver um pico inesperado de acessos no lançamento. |
| RF07 | Gerenciar perfil completo | Requisito "Should Have". O foco inicial deve ser no fluxo de adoção, a edição complexa de perfil pode aguardar. | Usuários não poderão alterar fotos ou preferências imediatamente. |

---

# 🔍 16. Revisão por Pares

**Grupo responsável pela revisão:** (A ser preenchido em sala pelo grupo revisor)

| ID do Requisito | Problema Encontrado | Sugestão de Melhoria |
|---|---|---|
| - | (Aguardando avaliação) | - |

---

# ✅ 17. Checklist de Qualidade dos Requisitos

- [X] Os requisitos estão completos?
- [X] Os requisitos estão corretos em relação às necessidades?
- [X] Cada requisito representa uma única capacidade ou característica?
- [X] Os requisitos são necessários?
- [X] Os requisitos são viáveis?
- [X] Todos possuem prioridade?
- [X] Termos ambíguos foram eliminados?
- [X] Os requisitos podem ser verificados ou testados?
- [X] A fonte ou stakeholder está identificado?
- [X] As necessidades estão relacionadas aos requisitos?
- [X] Os requisitos de qualidade são mensuráveis sempre que possível?
- [X] As prioridades MoSCoW possuem justificativa?

---

# 💭 18. Reflexão do Grupo

## 18.1 Qual requisito gerou mais discussão durante o levantamento? Por quê?
> A comunicação entre usuários (RF05). Discutimos se seria necessário um chat interno em tempo real ou apenas a disponibilização do contato (como WhatsApp) após o aceite do pedido, devido à complexidade de implementar um chat robusto.

## 18.2 Qual necessidade inicialmente parecia simples, mas gerou vários requisitos?
> O processo de adoção. Inicialmente parecia ser apenas um clique, mas desdobrou-se na necessidade de envio de pedido, aceite/recusa do doador, comunicação e regras de integridade (não excluir planta com pedido em andamento).

## 18.3 O grupo identificou algum requisito implícito durante a discussão?
> Sim, a necessidade de adequação à LGPD (RNF01) e a garantia de que as fotos inseridas fossem de tamanhos adequados para não prejudicar o desempenho (RNF03).

## 18.4 Qual requisito foi mais difícil de priorizar utilizando MoSCoW? Por quê?
> A avaliação de usuários (RF06). É um recurso muito importante para gerar segurança na comunidade, mas tecnicamente não é essencial para o fluxo básico (Minimum Viable Product), acabando classificado como "Could Have".

## 18.5 Houve algum requisito inicialmente considerado Must que mudou de prioridade?
> Sim, a edição detalhada do perfil (RF07). Percebemos que na primeira versão o usuário só precisa criar a conta e usar o sistema. A edição de dados não é bloqueante para a adoção em si, passando para "Should Have".

---

# 📝 19. Conclusão

> O projeto PlantTinder investigou a dificuldade de realizar a adoção responsável de plantas devido à falta de plataformas centralizadas. Identificamos que os principais stakeholders são os doadores e adotantes, cujas necessidades mais relevantes são um ambiente seguro para anunciar, buscar e gerenciar o processo de adoção. Os requisitos considerados essenciais (Must Have) focam exclusivamente na jornada principal: cadastro, anúncio, busca, pedido e comunicação. A técnica MoSCoW foi fundamental para evitar o excesso de escopo (scope creep), permitindo que o grupo separasse funcionalidades desejáveis (como sistema de avaliações e perfil complexo) das funcionalidades vitais para a primeira versão do sistema.

---

# 📚 Referência

REINEHR, Sheila. **Engenharia de Requisitos**. Bookman, 2020.

---
---

# 📑 FICHAS DE ELICITAÇÃO DE REQUISITOS (UDF)

---

## 📄 Ficha REQ-001 — Cadastro de Usuários

### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de autenticação, perfil e gerenciamento de acesso. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Todos os Usuários (Doadores e Adotantes) |
| Relação com o projeto | Usuário final |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes de plantas |
| Técnica e data da elicitação | Entrevista / Questionário (24/09/2026) |
| Responsável pelo registro | Davi Gonçalves Castro |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-001 (RF01) |
| Necessidade relatada pelo stakeholder | "Preciso me cadastrar na plataforma para poder doar ou adotar plantas de forma segura." |
| Descrição consolidada | O sistema deve permitir que novos usuários se cadastrem na plataforma fornecendo dados pessoais (nome, e-mail, senha, localização) e preferências de cultivo. |
| Justificativa ou benefício esperado | Garantir a identificação, rastreabilidade e segurança dos usuários na comunidade. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende de validação das diretrizes da LGPD (RNF01). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para acessar funções sensíveis. | RNF01 (Segurança) |
| RN-002 | O e-mail cadastrado deve ser único na plataforma. | Equipe de Desenvolvimento |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** Sem cadastro e autenticação, o sistema não possui controle de acesso nem segurança para os dados pessoais.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado que o usuário preencheu todos os campos obrigatórios válidos, quando clicar em "Cadastrar", então o sistema cria a conta e redireciona para a tela inicial. | Teste de cadastro com dados válidos e checagem no banco de dados. |
| CA-02 | Dado que o e-mail informado já está cadastrado, quando o usuário tentar finalizar o cadastro, então o sistema exibe mensagem de erro e impede o cadastro duplicado. | Teste unitário de e-mail duplicado. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Senhas devem ser armazenadas com criptografia (hash seguro). |
| Links relacionados | [GitHub - MF-DAVI](https://github.com/MF-DAVI) |

---

## 📄 Ficha REQ-002 — Anúncio de Plantas para Adoção

### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de gestão de anúncios de doação. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Doadores de Plantas (ST01) |
| Relação com o projeto | Usuário final (Doador) |
| Contato ou setor (se aplicável) | Doadores |
| Técnica e data da elicitação | Oficina / Entrevista (24/09/2026) |
| Responsável pelo registro | João Pedro Alves De Sousa |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-002 (RF02) |
| Necessidade relatada pelo stakeholder | "Quero cadastrar as plantas que tenho para doar com foto e detalhes dos cuidados que ela precisa." |
| Descrição consolidada | O sistema deve permitir que doadores cadastrem anúncios de plantas informando espécie, fotos, tamanho, cuidados específicos e localização de retirada. |
| Justificativa ou benefício esperado | Ofertar espécies na plataforma e esclarecer o nível de cuidado exigido antes do processo de adoção. |
| Tipo | Funcional |
| Dependências ou dúvidas | Requer estar autenticado (REQ-001). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Apenas usuários autenticados podem criar anúncios. | RNF01 |
| RN-003 | Uma planta cadastrada não pode ter campos obrigatórios (espécie, fotos e localização) em branco. | RNF05 (Integridade) |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** É a funcionalidade core da oferta. Sem plantas anunciadas, o sistema não possui catálogo para adoção.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um usuário autenticado com dados da planta preenchidos, quando submeter o anúncio, então o sistema publica a planta no catálogo. | Teste funcional de criação de postagem. |
| CA-02 | Dado um formulário de anúncio sem fotos anexadas, quando o doador tentar salvar, então o sistema bloqueia e exige pelo menos uma imagem. | Validação no frontend e backend. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Fotos devem passar por compressão para não degradar o tempo de carregamento (RNF03). |
| Links relacionados | [GitHub - jpedro-swe](https://github.com/jpedro-swe) |

---

## 📄 Ficha REQ-003 — Busca e Filtro de Plantas

### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de pesquisa, navegação e catálogo de anúncios. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Adotantes de Plantas (ST02) |
| Relação com o projeto | Usuário final (Adotante) |
| Contato ou setor (se aplicável) | Adotantes de plantas |
| Técnica e data da elicitação | Questionário / Análise de usabilidade (24/09/2026) |
| Responsável pelo registro | Hélter Brandão De Oliveira |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-003 (RF03) |
| Necessidade relatada pelo stakeholder | "Quero procurar plantas disponíveis perto da minha casa e filtrar por tamanho ou facilidade de cuidar." |
| Descrição consolidada | O sistema deve permitir que usuários busquem e filtrem plantas por espécie, porte/tamanho, localização e requisitos de cuidados. |
| Justificativa ou benefício esperado | Permitir que adotantes encontrem plantas adequadas à sua região e ao seu espaço disponível. |
| Tipo | Funcional |
| Dependências ou dúvidas | Pode requerer suporte à integração com API de geolocalização. |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-004 | Anúncios desativados ou com adoção concluída não devem aparecer nos resultados de busca pública. | Regra do Domínio |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** É a funcionalidade core da demanda. Permite o encontro entre o adotante e a planta desejada.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um filtro selecionado (ex: "Porte Pequeno"), quando o adotante pesquisar, então o sistema exibe apenas plantas correspondentes a esse critério. | Teste de integração de filtros no catálogo. |
| CA-02 | Dado um parâmetro de busca sem resultados, quando pesquisado, então o sistema exibe mensagem de "Nenhuma planta encontrada". | Verificação da interface e tratamento de lista vazia. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | O tempo de resposta da busca deve cumprir o limite estipulado em RNF03 (até 2s). |
| Links relacionados | [GitHub - brandao395](https://github.com/brandao395) |

---

## 📄 Ficha REQ-004 — Solicitação de Adoção

### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de gerenciamento do processo de adoção. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Adotantes e Doadores (ST01 e ST02) |
| Relação com o projeto | Usuários finais |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes |
| Técnica e data da elicitação | Oficina de Requisitos (24/09/2026) |
| Responsável pelo registro | Jorge Luis Soares do Santos |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-004 (RF04) |
| Necessidade relatada pelo stakeholder | "Quero mandar uma solicitação formal demonstrando interesse em adotar a planta para que o doador analise." |
| Descrição consolidada | O sistema deve permitir que um adotante autenticado envie um pedido de adoção para o doador de uma planta e que este doador aceite ou recuse a solicitação. |
| Justificativa ou benefício esperado | Formalizar e organizar o interesse, evitando interações desordenadas sobre o mesmo anúncio. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende de REQ-001 (autenticação) e REQ-002 (existência da planta). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para solicitar adoção. | RNF01 |
| RN-005 | Apenas o doador proprietário da planta pode aceitar ou rejeitar a solicitação. | RN03 / RNF05 |
| RN-006 | Uma planta com pedido de adoção pendente não pode ser removida do sistema. | RN02 / RNF05 |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** É a ação transacional do sistema (o "match") que formaliza o início do processo de transferência da planta.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um adotante interessado, quando ele clica em "Solicitar Adoção", então o sistema registra o pedido e notifica o doador. | Teste de fluxo transacional e notificação. |
| CA-02 | Dado um pedido em aberto, quando o doador clica em "Aceitar", então a solicitação muda de status para "Aprovada" e libera o canal de comunicação. | Teste de transição de status no pedido. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Múltiplos pedidos podem ser recebidos pelo doador antes do aceite. |
| Links relacionados | [GitHub - 7deo](https://github.com/7deo) |

---

## 📄 Ficha REQ-005 — Troca de Mensagens (Comunicação)

### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de mensagens e logística de entrega. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Todos os Usuários (Doadores e Adotantes) |
| Relação com o projeto | Usuários finais |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes |
| Técnica e data da elicitação | Entrevista / Análise documental (24/09/2026) |
| Responsável pelo registro | Davi Gonçalves Castro |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-005 (RF05) |
| Necessidade relatada pelo stakeholder | "Preciso conversar com a pessoa para combinar o dia, horário e local onde vou retirar ou entregar a planta." |
| Descrição consolidada | O sistema deve disponibilizar um canal interno de troca de mensagens entre o doador e o adotante após a solicitação de adoção. |
| Justificativa ou benefício esperado | Viabilizar o alinhamento logístico entre as partes garantindo privacidade de dados pessoais no contato inicial. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende da aceitação ou envio da solicitação (REQ-004). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para enviar mensagens. | RNF01 |
| RN-007 | O chat só pode ser iniciado entre doador e adotante atrelados a um pedido de adoção ativo. | Regra do Domínio |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** Sem comunicação, as partes não conseguem combinar a logística de retirada/entrega física da planta.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um pedido de adoção ativo, quando um dos usuários digita e envia uma mensagem, então ela deve ser entregue no painel do destinatário. | Teste de envio e recebimento de mensagens. |
| CA-02 | Dado um usuário não envolvido na adoção, quando tentar acessar a conversa alheia, então o acesso é negado. | Teste de permissão e segurança. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Na Versão 1 (MVP) será um chat básico assíncrono. |
| Links relacionados | [GitHub - MF-DAVI](https://github.com/MF-DAVI) |
