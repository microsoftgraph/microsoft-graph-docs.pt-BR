---
title: Visão geral da API de gráficos e pastas de trabalho do Excel
description: O Excel é uma ferramenta de produtividade indispensável. Os usuários de todos os setores e funções o usam como uma ferramenta para armazenar, acompanhar e manipular todos os tipos de dados. Ele é usado para tudo, desde de um simples acompanhamento de tarefas e gerenciamento de dados até cálculos complexos e relatórios profissionais. Você pode usar a API REST do Excel no Microsoft Graph para ampliar o valor de seus dados, cálculos, relatórios e painéis.
ms.localizationpriority: high
author: lumine2008
ms.prod: excel
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1380539804bdd4859385cc887a691b89b3e82965
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136107"
---
# <a name="excel-workbooks-and-charts-api-overview"></a>Visão geral da API de gráficos e pastas de trabalho do Excel

O Excel é uma ferramenta de produtividade indispensável. Os usuários de todos os setores e funções o usam como uma ferramenta para armazenar, acompanhar e manipular todos os tipos de dados. Ele é usado para tudo, desde de um simples acompanhamento de tarefas e gerenciamento de dados até cálculos complexos e relatórios profissionais. Você pode usar a API REST do Excel no Microsoft Graph para ampliar o valor de seus dados, cálculos, relatórios e painéis.

> [!VIDEO https://www.youtube-nocookie.com/embed/I1rSkJww2Dk]

## <a name="why-integrate-with-excel"></a>Por que integrar-se com o Excel?

Você pode usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive, no SharePoint ou em outras plataformas de armazenamento com suporte.

### <a name="perform-calculations"></a>Realizar cálculos

Os usuários adoram a facilidade com que eles podem realizar cálculos complexos e profundos no Excel. Agora, você pode acessar o avançado mecanismo de cálculo do Excel com resultados instantâneos. Por exemplo, uma calculadora de hipoteca pode utilizar a função PGTO do Excel ao realizar uma simples chamada de API que inclui o montante, a taxa e o número de pagamentos. O Excel faz o trabalho difícil e retorna o pagamento mensal instantaneamente. Com mais de 300 funções de planilha do Excel disponíveis, você tem acesso a todas as fórmulas oferecidas pelo Excel. Modelos de negócios complexos não precisam ser recriados várias vezes. Os desenvolvedores podem programar o Excel para realizar esses cálculos instantaneamente e recuperar os resultados com chamadas de API simples.

### <a name="generate-reports-and-analyze-results"></a>Gerar relatórios e analisar os resultados

O Excel é uma ferramenta flexível de análises e geração de relatórios, de tabelas de dados simples a complexos painéis profissionais. Hoje, oferecemos a você acesso total a todos os recursos de relatórios do Excel, tornando o Excel um serviço online de relatórios do Microsoft 365. Imagine qualquer cenário de relatório que os usuários criam e do qual dependem hoje transportado para um aplicativo personalizado que cria gráficos profissionais ou analisa grandes quantidades de dados de forma inteligente, integrando o Excel perfeitamente nessas experiências personalizadas.

### <a name="store-and-track-data"></a>Armazenar e acompanhar dados

O Excel também é uma ótima ferramenta para armazenar e acompanhar dados. Se suas informações são armazenadas em uma pasta de trabalho, esses dados estão disponíveis para qualquer aplicativo integrado ao Microsoft 365. Seu conteúdo está disponível para leitura de soluções personalizadas e essas soluções podem usar o Excel para armazenar dados.

>**Observação:** a API REST do Excel só oferece suporte para pastas de trabalho formatadas pelo arquivo do Office Open XML (arquivos com a extensão `.xlsx`). Não há suporte para pastas de trabalho de extensão `.xls`. 

### <a name="using-the-excel-rest-api"></a>Usar a API REST do Excel
Você pode usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive, no SharePoint ou em outras plataformas de armazenamento com suporte. O recurso `Workbook` (ou arquivo do Excel) contém todos os outros recursos do Excel por meio de relações. Você pode acessar uma pasta de trabalho por meio da API Drive identificando a localização do arquivo na URL. Por exemplo:

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`

`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`

Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho.

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API do Excel no Microsoft Graph v1.0](/graph/api/resources/excel?view=graph-rest-1.0)
- [API do Excel no Microsoft Graph beta](/graph/api/resources/excel?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

* [Gerenciar sessões do Excel usando o Microsoft Graph](excel-manage-sessions.md)
* [Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph](excel-write-to-workbook.md)
* [Usar funções de pasta de trabalho do Excel com o Microsoft Graph](excel-use-functions.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Exibir uma imagem do gráfico do Excel com o Microsoft Graph](excel-display-chart-image.md)
* [Usar a API REST do Excel](/graph/api/resources/excel?view=graph-rest-1.0)
