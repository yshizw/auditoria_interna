# Auditoria de Segurança da Informação

# Conteúdo

1. [Introdução](#introdução)
2. [Cenário](#cenário-e-escopo)
3. [Avaliação de Controles](#avaliação-de-controles)
4. [Compliance](#compliance)
5. [Relatório de recomendações](#relatório-de-recomendações)
6. [Conclusão](#conclusão)

--------

## Introdução

Este repositório apresenta um projeto pessoal de segurança da informação, no qual conduzi uma auditoria de segurança interna em uma empresa fictícia de nome "EcoBrindes".  

Utilizei um modelo de linguagem (LLM) para elaboração inicial do cenário e tomei como base a documentação presente no curso <a href='https://www.coursera.org/learn/manage-security-risks?specialization=cybersecurity-certificate'> Play It Safe: Manage Security Risks</a>, da Google. Desta forma, reestruturei o cenário para melhor aprendizado, evitando usar cenários prontos, e utilizei o português como linguagem para facilitar a leitura de partes interessadas. Possui o objetivo de simular, de forma mais fiel possível, um processo real de auditoria interna, incluindo a definição de escopo, objetivos, avaliação de riscos e a categorização de controles administrativos, técnicos e físicos.  

Esta simulação tem caráter educacional e foi elaborada como parte de meus estudos e projetos em cibersegurança, com foco no entedimento prático de frameworks de segurança, controles e conformidade.

## Cenário e Escopo

A EcoBrindes é uma empresa brasileira de pequeno porte que fabrica e vende brindes corporativos personalizados com foco em sustentabilidade. Com uma sede única, a empresa concentra em um só local suas operações administrativas, loja física, área de produção e estoque. Além disso, possui um e-commerce em crescimento, que ampliou o alcance da marca e trouxe novas demandas ao setor de tecnologia da informação (TI).  

Diante desse cenário de expansão, a equipe de TI identificou a necessidade de estabelecer um programa básico de segurança da informação, de modo a proteger os dados dos clientes, garantir a continuidade dos serviços e atender à Lei Geral de Proteção de Dados (LGPD). A gerente de TI decidiu, então, realizar uma auditoria interna, com o objetivo de mapear riscos, identificar vulnerabilidades e avaliar a efetividade dos controles existentes.  

O escopo da auditoria inclui os equipamentos de TI utilizados pelos colaboradores, a infraestrutura de rede interna da empresa e os sistemas que operam tanto na loja física quanto no e-commerce. Para orientar o processo, foi adotado o Framework de Cibersegurança do NIST (NIST CSF), por sua abordagem estruturada.  

A auditoria tem como foco principal diagnosticar a maturidade atual da segurança da informação na EcoBrindes, identificar oportunidades de melhoria e contribuir para o fortalecimento da governança de TI e da conformidade regulatória.  

_____

## Objetivos

Avaliar os ativos existentes e preencher o checklist de controles e conformidade para identificar quais medidas precisam ser adotadas para melhorar a segurança da EcoBrindes, entre eles:

- Verificar a conformidade com a Lei Geral de Proteção de Dados (LGPD)
- Avaliar a conformidade com o framework NIST CSF
- Melhorar os controles de segurança da informação
- Implementar o princípio do menor privilégio
- Avaliar a gestão e o inventário de ativos de TI
- Identificar e mitigar riscos operacionais e cibernéticos
- Verificar a eficácia dos backups e da continuidade de negócios
- Avaliar controles de acesso físico e lógico
- Conscientização em segurança entre os colaboradores

____



## Avaliação de Controles


Os ativos gerenciados pelo departamento de TI incluem:

- Computadores, impressoras, roteadores e switches usados no escritório
- Equipamentos dos funcionários: desktops, notebooks e smartphones para trabalho
- Produtos para venda na loja física e no e-commerce, armazenados no estoque
- Sistemas para controle de vendas, estoque e atendimento ao cliente (softwares locais e online)
- Rede interna simples e acesso à internet, sem segmentação
- Dados armazenados localmente em servidores, com backups feitos manualmente
- Sistema básico de câmeras de vigilância (CCTV) e fechaduras na loja física.  

Com base no "Controls and Compliance checklist", fornecido pela Google:

### Controles Administrativos/Gerenciais

| Nome do Controle      | Tipo do Controle      | Objetivo do Controle     | Necessidade de Implementação (Sim/Não)     | Prioridade     |
| -------------- | -------------- | -------------- | -------------- | -------------- |
| Menor privilégio   | Preventivo   | Reduzir riscos e impacto de colaboradores mal-intencionados ou contas comprometidas.  | Sim | Alta |
| Plano de recuperação de desastres   | Corretivo   | Garantir a continuidade dos negócios após incidentes.   | Sim | Alta |
| Política de senhas   | Preventivo   | Diminuir chances de comprometimento por ataques de força bruta ou dicionário.   | Sim | Alta |
| Política de controle de acesso   | Preventivo   | Garantir confidencialidade e integridade definindo quem pode acessar ou modificar dados.   | Sim | Alta |
| Política de gerenciamento de contas   | Preventivo   | Controlar o ciclo de vida das contas para reduzir superfície de ataque e limitar impacto de ex-funcionários.   | Sim | Alta |
| Separação de funções   | Preventivo   | Reduzir riscos e impacto de colaboradores mal-intencionados ou contas comprometidas.   | Sim | Alta |

### Controles Técnicos

| Nome do Controle      | Tipo do Controle      | Objetivo do Controle     | Necessidade de Implementação     | Prioridade     |
| -------------- | -------------- | -------------- | -------------- | -------------- |
| Firewall   | Preventivo   | Filtrar tráfego indesejado ou malicioso que tente entrar na rede.   | Não | Já implementado |
| IDS/IPS   | Detectivo   | Detectar e prevenir tráfego anômalo baseado em assinaturas ou regras.   | Sim | Alta |
| Criptografia   | Dissuasivo   | Garantir confidencialidade das informações sensíveis.   | Sim | Alta |
| Backups   | Corretivo   | Permitir restauração de dados após incidentes.   | Sim | Alta |
| Gerenciamento de senhas   | Preventivo   | Reduzir a fadiga e riscos relacionados ao uso e recuperação de senhas.   | Sim | Média/Alta |
| Antivírus   | Preventivo   | Detectar e isolar ameaças conhecidas.   | Sim | Alta |
| Manutenção   | Preventivo   | Identificar e gerenciar vulnerabilidades de sistemas desatualizados.   | Sim | Alta |

### Controles Físicos/Operacionais

| Nome do Controle      | Tipo do Controle      | Objetivo do Controle     | Necessidade de Implementação     | Prioridade     |
| -------------- | -------------- | -------------- | -------------- | -------------- |
| Cofre com controle de tempo   | Dissuasivo   | Reduzir superfície de ataque e impacto de ameaças físicas.   | Sim | Média |
| Iluminação adequada   | Dissuasivo   | Dificultar a ação de agentes maliciosos ao limitar locais escuros.   | Não | Já implementado |
| Câmeras de vigilância (CCTV)   | Preventivo/Detectivo   | Reduz risco de incidentes e possibilita investigação posterior.   | Não | Já implementado |
| Armários trancados (para equipamentos de rede)   | Preventivo   | Impedir acesso físico não autorizado aos equipamentos críticos.   | Sim | Alta |
| Placas indicando sistema de alarme   | Dissuasivo   | Tornar o ataque mais difícil e desencorajar invasores.   | Sim | Média |
| Trancas e fechaduras   | Dissuasivo/Preventivo   | Impedir acesso físico não autorizado a ativos.   | Não | Já implementado |
| Sistemas de detecção e prevenção de incêndio (alarme, sprinklers)   | Detectivo/Preventivo   | Detectar incêndios e prevenir danos a ativos físicos e estoque.   | Sim | Média/Alta |

____


## Compliance

Foram constatadas as seguintes necessidades de aderência:

#### Lei Geral de Proteção de Dados:

1. “O controlador deverá comunicar à autoridade nacional e ao titular a ocorrência de incidente de segurança que possa acarretar risco ou dano relevante aos titulares (...) em prazo razoável, conforme definido pela autoridade nacional”
- Necessidade de aderência ao artigo 48, informando ao cidadão caso tenha seus dados comprometidos.

2. "O RIPD é a documentação que contém a descrição dos processos de tratamento de dados pessoais que podem gerar alto risco à garantia dos princípios gerais de proteção de dados pessoais previstos na LGPD e às liberdades civis e aos direitos fundamentais do titular de dados. Deve conter, ainda, as medidas, salvaguardas e mecanismos de mitigação de risco"
- Implementar medidas, salvaguardas e mecanismos de mitigação de risco, de acordo com o princípio da Segurança da LGPD e seus artigos 5 e 38.

#### System and Organizations Controls (SOC tipo 1, SOC tipo 2)

*SOC 1 é uma auditoria dos controles internos em uma organização de serviço, implementada para proteger dados de propriedade do cliente que estão envolvidos no relatório financeiro do cliente.  
As auditorias do SOC 2 são baseadas nos Princípios e Critérios de Serviço de Confiança do AICPA para medir os controles internos da organização de serviços que são implementados para proteger dados de propriedade do cliente.*   

1. Aplicação de políticas de acesso, menor privilégio, separação de funções e gerenciamentos de contas.
- Necessidade de aderência visando confidencialidade de dados de clientes, restringindo e autorizando acesso apenas a funcionários designados.


___

## Relatório de recomendações

Esta auditoria interna evidenciou que a EcoBrindes, apesar de ser uma pequena empresa, apresenta lacunas importantes em sua gestão de segurança da informação e conformidade com a LGPD.

Recomendada aderência imediata à normas da LGPD (Lei Geral da Proteção de Dados), como separação de funções, gerenciamento de contas em seu sistema, políticas de controle de acesso e o princípio de menor privilégio, visto que a empresa EcoBrindes processa dados sensíveis de clientes e pagamentos. política de senhas para eficiência e segurança dos controles mencionados anteriormente.  

Se mostra crítica a necessidade de implementação de controles de segurança, tais como: update de Sistema imediato, implementação de IDS/IPS, criptografia em dados sensíveis, seguida de instalação de softwares antivírus para mitigação de riscos e vulnerabilidades. Planos para recuperação de desastres e backups também são prioridades visando continuidade de negócio. Firewall já implementado e em devido funcionamento pela equipe da EcoBrindes, com filtragem adequada. Gerenciamento de senhas, apesar de essencial, se faz menos crítica caso ocorra a implementação de funções mencionadas anteriormente, podendo ser realizada após.  

Prioridade também para o efetuamento de tranca em armários contendo sistemas de rede, para mitigar riscos relacionados à mesma. Devido a certos controles físicos já estarem em ação, é recomendado os seguintes controles adicionais: sprinklers e alarme de incêndio no local, placas sinalizando a presença de alarme para dissuasão de riscos de roubo, e cofre com controle de tempo para maior segurança.

____

## Conclusão

Desta forma, concluo meu projeto pessoal simulando uma auditoria interna de segurança da informação. Procurei utilizar o material base o mínimo possível, reformulando o material original e cenário fornecido pela Google, buscando uma absorção mais legítima e autêntica do conteúdo.  

*Lições aprendidas e desafios enfrentados:*

Acredito que a parte mais desafiadora foi a avaliação das prioridades dos controles a serem implementados. Algumas medidas são claramente urgentes, mas foi necessário um esforço maior para identificar com precisão aquelas que realmente demandam atenção imediata, ao invés de simplesmente marcar prioridade alta em todas.

Esta simulação teve como objetivo aprofundar meus conhecimentos sobre os tipos de controle, a Lei Geral de Proteção de Dados (LGPD), os princípios do NIST, entre outros temas relacionados à segurança da informação, além de proporcionar um insight prático na estruturação de uma auditoria interna.

Feedbacks e sugestões são bem-vindos.