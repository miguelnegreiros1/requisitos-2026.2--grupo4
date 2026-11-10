# Visão da Demanda (VD)

## Histórico de Versões

| Data       | Versão | Descrição                                                        | Autor        |
| ---------- | ------ | ---------------------------------------------------------------- | ------------ |
| 03/11/2026 | 1.0    | Criação inicial do documento de visão para a Plataforma de Gestão de Oportunidades Acadêmicas Internacionais | Miguel Rodrigues |
| 10/11/2026 | 1.1    | Restrição de escopo e público-alvo focados exclusivamente nos estudantes de graduação da UNIFOR e adição/organização de requisitos | Miguel Rodrigues |

## 1. Objetivo

Definir a proposta de valor e o escopo da **Plataforma de Gestão de Oportunidades Acadêmicas Internacionais**, detalhando as necessidades dos estudantes de graduação da **UNIFOR**, da Diretoria de Relações Internacionais (DRI), das universidades estrangeiras parceiras e dos coordenadores de curso.

## 2. Proposta de Valor

O sistema permitirá modernizar, organizar e dar maior visibilidade aos editais, bolsas e oportunidades de mobilidade internacional promovidos pela UNIFOR. Inspirada em redes sociais profissionais (estilo LinkedIn), a plataforma tornará a busca intuitiva e engajadora para os alunos da instituição, automatizando a validação de requisitos institucionais e o acompanhamento de manifestações de interesse, o que reduz burocracias e amplia a transparência para toda a comunidade acadêmica da UNIFOR.

## 3. Descrição da Demanda

A demanda consiste no desenvolvimento de um ecossistema digital integrado para gerenciar o ciclo de vida da internacionalização acadêmica no âmbito da UNIFOR. O sistema apoiará a DRI no cadastro centralizado de editais e bolsas, as universidades estrangeiras na divulgação de vagas e critérios específicos, e os estudantes de graduação da UNIFOR na descoberta personalizada de oportunidades com base em seus perfis acadêmicos. O processo incluirá feed de notícias, filtros avançados, checagem automatizada de elegibilidade e acompanhamento em tempo real das candidaturas.

## 4. Partes Interessadas

| Nome                         | Papel           | Responsabilidades                                   | Representante           |
|------------------------------|-----------------|-----------------------------------------------------|-------------------------|
| Diretoria de Relações Internacionais (DRI) | Cliente / Gestor | Cadastrar editais, aprovar vagas, gerenciar prazos e emitir diretrizes de mobilidade | Dra. Gina Pompeu           |
| Estudantes de Graduação da UNIFOR | Usuário Final   | Buscar oportunidades, verificar elegibilidade, submeter documentação e acompanhar status | -                       |
| Universidades Estrangeiras Parceiras | Stakeholder Externo | Disponibilizar vagas, definir requisitos linguísticos e acadêmicos e receber os alunos | Instituições Parceiras  |
| Coordenadores de Curso       | Stakeholder Indireto | Acompanhar alunos em mobilidade e apoiar equivalências de disciplinas | -                       |
| Equipe de TI / Desenvolvimento | Desenvolvimento | Desenvolver, implantar e manter a infraestrutura técnica do sistema | Miguel Rodrigues         |

## 5. Personas

### 5.1. Estudante de Graduação da UNIFOR (Ex: João, 5º semestre)
- **Descrição:** Aluno regularmente matriculado na UNIFOR, elegível (com 30% a 70% do curso concluído, média global $\ge 7,0$ e sem reprovações) que sonha em fazer intercâmbio, mas acha difícil acompanhar os editais espalhados em portais institucionais.
- **Objetivo:** Encontrar oportunidades alinhadas ao seu perfil em um feed dinâmico, validar sua elegibilidade de forma rápida e candidatar-se sem fricção.

### 5.2. Gestor do Núcleo de Estratégias Internacionais (Ex: Maria do DRI)
- **Descrição:** Servidora responsável por gerenciar as parcerias internacionais e divulgar os editais de bolsas da UNIFOR.
- **Objetivo:** Cadastrar editais de forma centralizada, acompanhar o volume de manifestações de interesse e otimizar a comunicação com os alunos candidatos.

---

## 6. Regras de Negócio (RN)

- **RN01 - Restrição de Acesso Institucional:** O acesso à plataforma e a submissão de candidaturas são restritos exclusivamente a estudantes de graduação regularmente matriculados na UNIFOR, autenticados via credenciais institucionais.
- **RN02 - Critério de Elegibilidade Acadêmica:** O aluno só é elegível a candidatar-se caso possua entre 30% e 70% da carga horária concluída, média geral/IRA $\ge 7,0$ e zero reprovações em seu histórico acadêmico.
- **RN03 - Imutabilidade de Dados Oficiais:** O aluno não pode editar manualmente suas notas, percentual de curso concluído ou histórico de reprovações; esses dados devem ser oriundos exclusivamente do sistema acadêmico oficial da UNIFOR.
- **RN04 - Limite de Inscrições Ativas:** Um estudante só pode ter no máximo **3** manifestações de interesse/candidaturas ativas simultaneamente em editais abertos.
- **RN05 - Prazo Limite para Submissão:** Candidaturas e envios de documentação enviados após às 23h59 (horário de Brasília) da data de encerramento do edital devem ser rejeitados automaticamente pelo sistema.

## 7. Necessidades e Funcionalidades

### Necessidade 1: Divulgação e Descoberta de Oportunidades (Estilo Rede Social)

#### F1.1 Feed Dinâmico de Oportunidades
- **Descrição:** Exibe um feed personalizado na página inicial com postagens recentes, editais em destaque e recomendações com base no curso e histórico do aluno da UNIFOR.
- **Atores:** Estudantes de Graduação da UNIFOR
- **Frequência:** Alta
- **Valor:** Alto

#### F1.2 Filtros de Busca Avançada
- **Descrição:** Permite buscar oportunidades filtrando por país, universidade parceira, área de conhecimento, tipo de bolsa e prazo de inscrição.
- **Atores:** Estudantes de Graduação da UNIFOR
- **Frequência:** Alta
- **Valor:** Alto

---

### Necessidade 2: Gestão Institucional de Editais e Vagas

#### F2.1 Cadastro e Edição de Editais
- **Descrição:** Permite a DRI cadastrar novos editais voltados para a comunidade acadêmica da UNIFOR, especificando prazos, requisitos, número de vagas e documentação exigida.
- **Atores:** DRI
- **Frequência:** Média
- **Valor:** Alto

#### F2.2 Integração com Requisitos de Universidades Estrangeiras
- **Descrição:** Permite vincular as vagas às exigências específicas das universidades parceiras (ex: proficiência em idiomas).
- **Atores:** DRI, Universidades Estrangeiras
- **Frequência:** Baixa
- **Valor:** Médio

---

### Necessidade 3: Validação de Elegibilidade e Submissão

#### F3.1 Cadastro e Gestão de Perfil do Estudante
- **Descrição:** Permite ao estudante da UNIFOR gerenciar seu perfil na plataforma. O sistema importa automaticamente os dados oficiais do sistema acadêmico da UNIFOR e permite complementar o perfil com foto, resumo/biografia, proficiência em idiomas e áreas de interesse.
- **Atores:** Estudante da UNIFOR, Sistema Acadêmico da UNIFOR
- **Frequência:** Alta
- **Valor:** Alto

#### F3.2 Verificação Automática de Elegibilidade
- **Descrição:** Cruzamento automático dos dados acadêmicos do aluno da UNIFOR com as regras do edital (conforme RN02) para sinalizar se ele está apto a concorrer.
- **Atores:** Sistema, Estudante
- **Frequência:** Alta
- **Valor:** Alto

#### F3.3 Manifestação de Interesse e Acompanhamento
- **Descrição:** Permite ao estudante enviar a documentação necessária e acompanhar o status de sua candidatura em tempo real (respeitando a restrição de limite de candidaturas ativas).
- **Atores:** Estudante, DRI
- **Frequência:** Alta
- **Valor:** Alto

---
- **Descrição:** Proteção rigorosa de dados pessoais e históricos acadêmicos dos estudantes da UNIFOR armazenados na plataforma, alinhada às políticas de privacidade institucionais.
- **Atores:** Administração de TI
- **Frequência:** Sempre
- **Valor:** Alto
