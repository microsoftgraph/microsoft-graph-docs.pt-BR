---
title: Visão geral da API Microsoft Search no Microsoft Graph (visualização)
description: Use a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 6f7515682f7600a4c0d58e49213eacf17add44e0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866893"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a>Visão geral da API Microsoft Search no Microsoft Graph (visualização)

A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização. Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados. A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing. Você pode usar a API de pesquisa da Microsoft no Microsoft Graph para estender a pesquisa da Microsoft para seus aplicativos.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Por que usar a API de Pesquisa da Microsoft?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft

A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa que você pode usar para permitir que os desenvolvedores [consultem](/graph/api/search-query?view=graph-rest-beta) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.

### <a name="include-custom-external-data-in-search-experience"></a>Incluir dados externos personalizados na experiência de pesquisa

Os clientes que queiram incluir dados que estejam fora da nuvem da Microsoft em suas pesquisas poderão usar [conectores](/microsoftsearch/connectors-overview) que se conectem a uma fonte de dados específica, como um banco de dados de recursos humanos ou catálogo de produtos da organização. Para [consultar](/graph/api/search-query?view=graph-rest-beta) diretamente a fonte de dados externa, use a API de Pesquisa da Microsoft. A [Galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) lista vários conectores prontos para uso. Como alternativa, os clientes podem [criar conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexar arquivos e itens personalizados externos e consultar fontes de dados externas específicas.

### <a name="consistent-up-to-date-search-experience"></a>Experiência de pesquisa atualizada e consistente

Ao usar a API de pesquisa da Microsoft, seus clientes se beneficiam dos resultados de pesquisa relevantes mais personalizados com a plataforma Microsoft Graph. A experiência de pesquisa em seus aplicativos retorna resultados que são consistentes com a pesquisa em aplicativos do Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Quais dados posso adicionar ou acessar usando a API de pesquisa da Microsoft?

A API de pesquisa da Microsoft suporta para pesquisar o seguinte conteúdo na nuvem da Microsoft:

- Objetos [message](/graph/api/resources/message?view=graph-rest-beta) e [event](/graph/api/resources/event?view=graph-rest-beta) do Outlook
- Objetos de arquivos [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) do SharePoint e do OneDrive

Além disso, você pode indexar e pesquisar conteúdos externos, por meio do seguinte:

- Objetos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) que são de tipos personalizados
- Objetos [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) que são de tipos conhecidos

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [Usar a API de Pesquisa da Microsoft para indexar dados](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).
- Saiba mais sobre alguns dos principais casos de uso:
  - [Pesquisar mensagens do Outlook](search-concept-messages.md)
  - [Pesquisar eventos do calendário](search-concept-events.md)
  - [Gerenciar conexões para indexar conteúdo externo](search-index-manage-connections.md)
  - [Indexar conteúdo externo](search-index-manage-items.md)
  - [Pesquisar tipos personalizados (externalItem)](search-concept-custom-types.md)
  - [Pesquisar arquivos (incluindo externalFile)](search-concept-files.md)
- Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.

## <a name="see-also"></a>Confira também

- Entre em contato com a Comunidade no [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-search).
