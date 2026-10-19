# Projetos em destaque — contexto técnico

Este documento apresenta problemas abordados, decisões técnicas observáveis no código e limitações atuais dos projetos públicos do portfólio. Não são alegadas métricas de produção ou resultados que ainda não foram medidos.

## 1. [ERP Costuras Hoinatz](https://github.com/Kaue-Borges/erp-costuras-hoinatz)

**Objetivo:** concentrar rotinas de produção de uma confecção em uma aplicação web organizada.

**O que foi construído:** interface React + TypeScript com navegação por módulos de cadastros, ordens de produção, apontamentos, indicadores e geração de etiquetas. O processamento de documentos PDF usa PDF.js, com regras de interpretação por fornecedor.

**Competências demonstradas:**
- Componentização e roteamento de telas em React.
- Modelagem de entidades e operações CRUD no frontend.
- Separação entre componentes, páginas, repositórios e serviços.
- Extração de informação de PDFs e regras de cálculo de produção.

**Limitação real:** o armazenamento desta versão é feito em `localStorage`; ela não implementa banco de dados centralizado ou emissão fiscal integrada. Próxima evolução técnica: persistência segura, autenticação, testes e CI.

**Onde conferir:** [código-fonte e instruções](https://github.com/Kaue-Borges/erp-costuras-hoinatz).

## 2. [Automação de produtos WooCommerce](https://github.com/Kaue-Borges/woocommerce-product-automation)

**Objetivo:** reduzir tarefas manuais repetitivas relacionadas à gestão das mídias de produtos no WooCommerce.

**O que foi construído:** scripts Python com Playwright para localizar produtos por SKU e gerenciar arquivos de mídia, com painéis locais em Flask para processamento em lote e acompanhamento de resultados. Há também um módulo de remoção de mídias, que exige cuidado por modificar registros reais.

**Competências demonstradas:**
- Automação de interfaces web e tratamento de fluxos por SKU.
- Backend local com Flask e endpoints de acompanhamento.
- Leitura e classificação de arquivos em diretórios.
- Rotinas em lote e tratamento de erros.

**Limitação real:** a estrutura tem duplicação entre versões do dashboard e configurações locais ainda acopladas ao código. Próximos passos: configuração por ambiente, testes com mocks e pipeline de verificação offline.

**Onde conferir:** [código-fonte e documentação](https://github.com/Kaue-Borges/woocommerce-product-automation).

## 3. [Aulas da Faculdade](https://github.com/Kaue-Borges/aulas-faculdade)

**Objetivo:** organizar a evolução acadêmica em uma estrutura acessível por disciplina, em vez de manter diversos repositórios pequenos.

**O que foi construído:** acervo de exercícios em C++, Java, HTML/CSS/JavaScript e Node.js/Express, distribuído por semestre, matéria e projeto. O código inclui exercícios de programação orientada a objetos e pequenos exemplos de APIs.

**Competências demonstradas:**
- Fundamentos de programação e modelagem com classes.
- Exercícios frontend e manipulação de eventos.
- Criação de endpoints e noções de APIs em Node.js/Express.
- Organização e documentação de repositórios Git.

**Limitação real:** é um acervo de trabalhos acadêmicos, não um sistema único. Alguns exercícios exigem testes e ajustes próprios.

**Onde conferir:** [índice das disciplinas](https://github.com/Kaue-Borges/aulas-faculdade).

## 4. DevOps & Cloud — laboratório em evolução

Existe um laboratório separado com **Docker, Nginx e workflows GitHub Actions**. Ele permanece privado enquanto o conteúdo e as configurações são revisados. Não é apresentado como repositório público nem como ambiente de produção.

**Foco de evolução:** automatizar builds e verificações de projetos públicos, aprofundar Linux, redes, infraestrutura como código e observabilidade.

---

Atualizado como documentação de portfólio. A implementação efetiva e as limitações devem sempre ser conferidas nos repositórios de origem.
