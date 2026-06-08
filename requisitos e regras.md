# Documento de Levantamento de Requisitos

## Sistema de Gerenciamento de Portarias

### Instituto Federal Catarinense – Campus Videira

---

# 1. Introdução

## 1.1 Objetivo

Este documento tem como objetivo apresentar o levantamento inicial de requisitos para o desenvolvimento de um Sistema de Gerenciamento de Portarias destinado ao Instituto Federal Catarinense – Campus Videira. O sistema visa apoiar os processos administrativos relacionados à solicitação, elaboração, emissão, acompanhamento, vigência e arquivamento de portarias institucionais.

### Link do Protótipo

O protótipo do sistema foi desenvolvido no Figma e pode ser acessado pelo link abaixo:

[Landing Page no figma](https://www.figma.com/design/HxLNnzBS1dfCG7NGcLBOBB/Landing_Page-Gestor_Portarias?node-id=1-136&t=NAKeVfRCCEPkHkjF-1)

---

## 1.2 Contextualização

O Instituto Federal Catarinense – Campus Videira atua na oferta de educação técnica, tecnológica, superior e de pós-graduação, atendendo diferentes modalidades de ensino e níveis de formação. Dentro de sua estrutura organizacional, destacam-se os seguintes setores administrativos:

* Direção Geral (DG);
* Diretoria de Administração e Planejamento (DAP);
* Diretoria de Ensino, Pesquisa e Extensão (DEPE);
* Gabinete Institucional;
* Coordenação de Gestão de Pessoas (CGP).

Atualmente, a gestão de portarias é realizada de maneira predominantemente manual, ocasionando dificuldades relacionadas ao controle de documentos, acompanhamento de vigência, rastreabilidade de alterações, distribuição de responsabilidades e emissão de relatórios administrativos.

Dessa forma, propõe-se o desenvolvimento de uma solução informatizada capaz de centralizar e automatizar o fluxo de gerenciamento de portarias institucionais.

---

# 2. Descrição Geral do Sistema

O sistema deverá permitir o gerenciamento completo do ciclo de vida das portarias institucionais, compreendendo:

* Solicitação de portarias;
* Validação administrativa;
* Emissão e assinatura;
* Controle de membros;
* Controle de carga horária;
* Monitoramento de vigência;
* Histórico de alterações;
* Emissão de relatórios;
* Integração futura com sistemas institucionais.

Além disso, o sistema deverá oferecer diferentes níveis de acesso conforme os perfis administrativos e funcionais dos usuários envolvidos.

---

# 3. Regras de Negócio

## RN01 — Emissão de Portarias

Somente os setores Gabinete Institucional e Coordenação de Gestão de Pessoas poderão emitir portarias institucionais.

---

## RN02 — Assinatura de Portarias

Somente o Diretor Geral do campus ou seu Vice-Diretor oficialmente designado poderão realizar a assinatura de portarias.

---

## RN03 — Tipos de Portaria

O sistema deverá suportar os seguintes tipos de portarias:

* Nova Portaria;
* Portaria de Revogação;
* Portaria Normativa.

---

## RN04 — Relacionamento com Memorandos

Uma portaria poderá estar associada a nenhum, um ou múltiplos memorandos institucionais.

---

## RN05 — Solicitação de Portarias

Servidores docentes e técnicos administrativos poderão solicitar a criação de portarias mediante justificativa formal.

---

## RN06 — Participação Externa

O sistema deverá permitir a inclusão de membros externos, alunos e comunidade geral nas portarias institucionais.

Para membros externos deverão ser obrigatórios:

* Nome completo;
* CPF.

---

## RN07 — Controle de Vigência

Toda portaria deverá possuir:

* Data de início;
* Data de término ou período de vigência;
* Situação atual.

---

## RN08 — Notificação Automática

Após a assinatura da portaria, os membros vinculados deverão receber comunicação automática via correio eletrônico, contendo o documento oficial em anexo.

---

## RN09 — Histórico de Alterações

O sistema deverá manter histórico completo de alterações realizadas nas portarias, permitindo rastreabilidade e recuperação de versões anteriores.

---

## RN10 — Controle de Perfis de Acesso

O sistema deverá implementar controle de acesso baseado em perfis de usuário.

---

## RN11 — Cadastro Obrigatório de Usuários

Os usuários internos deverão possuir cadastro contendo obrigatoriamente:

* Nome;
* CPF;
* SIAP;
* Órgão;
* Departamento;
* Cargo;
* Telefone;
* E-mail;
* Endereço;
* Chefia imediata.

---

## RN12 — Controle de Carga Horária

Os membros vinculados às portarias deverão possuir registro de carga horária semanal associada às respectivas atividades.

---

## RN13 — Monitoramento de Vigência

O sistema deverá monitorar automaticamente os períodos de vigência das portarias, emitindo alertas de renovação ou encerramento.

---

## RN14 — Estados da Portaria

As portarias deverão possuir os seguintes estados:

* Em edição;
* Em validação;
* Assinada;
* Em vigência;
* Revogada;
* Atualizada;
* Encerrada.

---

# 4. Requisitos Funcionais

## RF01 — Cadastro de Usuários

O sistema deverá permitir o cadastro de usuários institucionais.

---

## RF02 — Autenticação

O sistema deverá permitir autenticação mediante login e senha.

---

## RF03 — Controle de Permissões

O sistema deverá controlar permissões conforme o perfil do usuário.

---

## RF04 — Gerenciamento de Usuários

O administrador deverá poder habilitar ou desabilitar usuários.

---

## RF05 — Criação de Portarias

O sistema deverá permitir a criação de novas portarias.

---

## RF06 — Edição de Portarias

O sistema deverá permitir a edição de portarias em elaboração.

---

## RF07 — Revogação de Portarias

O sistema deverá permitir revogação de portarias existentes.

---

## RF08 — Atualização de Portarias

O sistema deverá permitir atualização de informações de portarias vigentes.

---

## RF09 — Associação de Memorandos

O sistema deverá permitir anexar memorandos relacionados às portarias.

---

## RF10 — Cadastro de Membros

O sistema deverá permitir cadastrar membros vinculados às portarias.

---

## RF11 — Definição de Carga Horária

O sistema deverá permitir informar carga horária semanal dos membros.

---

## RF12 — Definição de Vigência

O sistema deverá permitir definir período de vigência das portarias.

---

## RF13 — Numeração Automática

O sistema deverá gerar automaticamente a numeração das portarias.

---

## RF14 — Geração de Documento

O sistema deverá gerar documento oficial em formato PDF.

---

## RF15 — Assinatura Digital

O sistema deverá permitir assinatura digital das portarias.

---

## RF16 — Consulta de Portarias

O sistema deverá permitir consulta de portarias cadastradas.

---

## RF17 — Busca Avançada

O sistema deverá permitir buscas por:

* Número;
* Ano;
* Servidor;
* Tipo;
* Status;
* Departamento.

---

## RF18 — Histórico de Alterações

O sistema deverá permitir visualização do histórico de alterações.

---

## RF19 — Versionamento

O sistema deverá armazenar versões anteriores das portarias.

---

## RF20 — Solicitação de Portarias

O sistema deverá permitir submissão de solicitações de portarias.

---

## RF21 — Validação Administrativa

O sistema deverá permitir validação administrativa das solicitações.

---

## RF22 — Aprovação ou Rejeição

O sistema deverá permitir aprovação ou rejeição das solicitações.

---

## RF23 — Registro de Justificativas

O sistema deverá registrar justificativas em casos de rejeição.

---

## RF24 — Notificações Automáticas

O sistema deverá enviar notificações automáticas por e-mail.

---

## RF25 — Alertas de Vencimento

O sistema deverá emitir alertas de vencimento de portarias.

---

## RF26 — Relatórios Gerenciais

O sistema deverá gerar:

* Relatório de servidores por portaria;
* Relatório de carga horária;
* Relatório anual de portarias por status.

---

## RF27 — Exportação de Relatórios

O sistema deverá permitir exportação de relatórios em PDF.

---

## RF28 — Integração Externa

O sistema deverá prever integração futura com sistemas institucionais, como o SIPAC.

---

# 5. Requisitos Não Funcionais

## RNF01 — Segurança

O sistema deverá possuir mecanismos de autenticação e autorização de acesso.

---

## RNF02 — Auditoria

O sistema deverá registrar logs de auditoria das operações realizadas.

---

## RNF03 — Integridade

O sistema deverá garantir integridade dos documentos assinados digitalmente.

---

## RNF04 — Desempenho

Consultas ao sistema deverão possuir tempo de resposta inferior a três segundos.

---

## RNF05 — Disponibilidade

O sistema deverá possuir disponibilidade mínima de 99%.

---

## RNF06 — Backup

O sistema deverá realizar backups automáticos periódicos.

---

## RNF07 — Responsividade

O sistema deverá possuir interface responsiva compatível com dispositivos móveis.

---

## RNF08 — Compatibilidade

O sistema deverá ser compatível com os navegadores:

* Google Chrome;
* Microsoft Edge;
* Mozilla Firefox.

---

## RNF09 — Escalabilidade

O sistema deverá permitir expansão modular futura.

---

## RNF10 — Integração via API

O sistema deverá disponibilizar API REST para integrações futuras.

---

## RNF11 — Conformidade Legal

O sistema deverá atender às diretrizes da Lei Geral de Proteção de Dados (LGPD).

---

# 6. Considerações Finais

O levantamento de requisitos apresentado constitui a base inicial para o desenvolvimento do Sistema de Gerenciamento de Portarias do Instituto Federal Catarinense – Campus Videira.

Os requisitos identificados servirão como subsídio para as próximas etapas do projeto, incluindo modelagem de processos, modelagem de dados, prototipação de interfaces, arquitetura de software e implementação do sistema.
