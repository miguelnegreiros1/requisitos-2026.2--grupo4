# Visão da Demanda (VD)

## Histórico de Versões

| Data       | Versão | Descrição                                                        | Autor        |
| ---------- | ------ | ---------------------------------------------------------------- | ------------ |
| 03/11/2026 | 1.0    | Criação inicial do documento de visão para a Plataforma de Gestão de Oportunidades Acadêmicas Internacionais | Miguel Rodrigues |

## 1. Objetivo

Definir a proposta de valor e o escopo da **Plataforma de Gestão de Oportunidades Acadêmicas Internacionais**, detalhando as necessidades dos estudantes de graduação, do Núcleo de Estratégias Internacionais (NEI), das universidades estrangeiras parceiras e dos coordenadores de curso.

## 2. Proposta de Valor

O sistema permitirá modernizar, organizar e dar maior visibilidade aos editais, bolsas e oportunidades de mobilidade internacional promovidos pela instituição. Inspirada em redes sociais profissionais (estilo LinkedIn), a plataforma tornará a busca intuitiva e engajadora, automatizando a validação de requisitos e o acompanhamento de manifestações de interesse, o que reduz burocracias e amplia a transparência para toda a comunidade acadêmica.

## 3. Descrição da Demanda

A demanda consiste no desenvolvimento de um ecossistema digital integrado para gerenciar o ciclo de vida da internacionalização acadêmica. O sistema apoiará o NEI no cadastro centralizado de editais e bolsas, as universidades estrangeiras na divulgação de vagas e critérios específicos, e os estudantes na descoberta personalizada de oportunidades com base em seus perfis acadêmicos. O processo incluirá feed de notícias, filtros avançados, checagem automatizada de elegibilidade e acompanhamento em tempo real das candidaturas.

## 4. Partes Interessadas

| Nome                         | Papel           | Responsabilidades                                   | Representante           |
|------------------------------|-----------------|-----------------------------------------------------|-------------------------|
| Núcleo de Estratégias Internacionais (NEI) | Cliente / Gestor | Cadastrar editais, aprovar vagas, gerenciar prazos e emitir diretrizes de mobilidade | Equipe do NEI           |
| Estudantes de Graduação      | Usuário Final   | Buscar oportunidades, verificar elegibilidade, submeter documentação e acompanhar status | -                       |
| Universidades Estrangeiras Parceiras | Stakeholder Externo | Disponibilizar vagas, definir requisitos linguísticos e acadêmicos e receber os alunos | Instituições Parceiras  |
| Coordenadores de Curso       | Stakeholder Indireto | Acompanhar alunos em mobilidade e apoiar equivalências de disciplinas | -                       |
| Equipe de TI / Desenvolvimento | Desenvolvimento | Desenvolver, implantar e manter a infraestrutura técnica do sistema | Equipe do Projeto       |

## 5. Personas

### 5.1. Estudante de Graduação (Ex: João, 5º semestre)
- **Descrição:** Aluno elegível (com 30% a 70% do curso concluído, média global $\ge 7,0$ e sem reprovações) que sonha em fazer intercâmbio, mas acha difícil acompanhar os editais espalhados em portais institucionais.
- **Objetivo:** Encontrar oportunidades alinhadas ao seu perfil em um feed dinâmico, validar sua elegibilidade de forma rápida e candidatar-se sem fricção.

### 5.2. Gestor do Núcleo de Estratégias Internacionais (Ex: Maria do NEI)
- **Descrição:** Servidora responsável por gerenciar as parcerias internacionais e divulgar os editais de bolsas.
- **Objetivo:** Cadastrar editais de forma centralizada, acompanhar o volume de manifestações de interesse e otimizar a comunicação com os alunos candidatos.

---

## 6. Necessidades e Funcionalidades

### Necessidade 1: Divulgação e Descoberta de Oportunidades (Estilo Rede Social)

#### F1.1 Feed Dinâmico de Oportunidades
- **Descrição:** Exibe um feed personalizado na página inicial com postagens recentes, editais em destaque e recomendações com base no curso e histórico do aluno.
- **Status:** Incluída
- **Atores:** Estudantes de Graduação
- **Frequência:** Alta
- **Valor:** Alto

#### F1.2 Filtros de Busca Avançada
- **Descrição:** Permite buscar oportunidades filtrando por país, universidade parceira, área de conhecimento, tipo de bolsa e prazo de inscrição.
- **Status:** Incluída
- **Atores:** Estudantes de Graduação
- **Frequência:** Alta
- **Valor:** Alto

---

### Necessidade 2: Gestão Institucional de Editais e Vagas

#### F2.1 Cadastro e Edição de Editais
- **Descrição:** Permite ao NEI cadastrar novos editais, especificando prazos, requisitos, número de vagas e documentação exigida.
- **Status:** Incluída
- **Atores:** NEI
- **Frequência:** Média
- **Valor:** Alto

#### F2.2 Integração com Requisitos de Universidades Estrangeiras
- **Descrição:** Permite vincular as vagas às exigências específicas das universidades parceiras (ex: proficiência em idiomas).
- **Status:** Incluída
- **Atores:** NEI, Universidades Estrangeiras
- **Frequência:** Baixa
- **Valor:** Médio

---

### Necessidade 3: Validação de Elegibilidade e Submissão

#### F3.3 Cadastro e Gestão de Perfil do Estudante
- **Descrição:** Permite ao estudante criar e gerenciar seu perfil na plataforma. O sistema deve carregar automaticamente os dados acadêmicos oficiais do sistema institucional (curso, média global/IRA, % de carga horária concluída e histórico de reprovações) e permitir que o aluno complemente o perfil com foto, resumo/biografia, proficiência em idiomas e áreas de interesse para recomendação de oportunidades.
- **Incluída**
- **Atores:** Estudante de Graduação, Sistema Institucional
- **Frequência:** Alta
- **Valor:** Alto

#### F3.2 Verificação Automática de Elegibilidade
- **Descrição:** Cruzamento automático dos dados acadêmicos do aluno (ex: média global e percentual concluído) com as regras do edital para sinalizar se ele está apto a concorrer.
- **Status:** Incluída
- **Atores:** Sistema, Estudante
- **Frequência:** Alta
- **Valor:** Alto

#### F3.3 Manifestação de Interesse e Acompanhamento
- **Descrição:** Permite ao estudante enviar a documentação necessária e acompanhar o status de sua candidatura em tempo real (em análise, aprovado, pendente).
- **Status:** Incluída
- **Atores:** Estudante, NEI
- **Frequência:** Alta
- **Valor:** Alto

---

### Necessidade 4: Requisitos Não Funcionais (Segurança, Desempenho e Qualidade)

#### F4.1 Usabilidade e Design Responsivo
- **Descrição:** A interface deve ser fluida e amigável (inspirada no LinkedIn), funcionando perfeitamente em computadores e dispositivos móveis.
- **Status:** Incluída
- **Atores:** Todos os usuários
- **Frequência:** Sempre
- **Valor:** Alto

#### F4.2 Desempenho do Sistema
- **Descrição:** O feed e as buscas de editais devem carregar em até 2 segundos, mesmo em períodos de pico de inscrições.
- **Status:** Incluída
- **Atores:** Todos
- **Frequência:** Sempre
- **Valor:** Alto

#### F4.3 Segurança e Privacidade de Dados (LGPD)
- **Descrição:** Proteção rigorosa de dados pessoais e históricos acadêmicos dos estudantes armazenados na plataforma.
- **Status:** Incluída
- **Atores:** Administração de TI
- **Frequência:** Sempre
- **Valor:** Alto
