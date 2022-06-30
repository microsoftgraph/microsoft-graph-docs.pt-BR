---
title: Visão geral da API de Pesquisa da Microsoft no Microsoft Graph
description: Use a API de Pesquisa da Microsoft no Microsoft Graph para estender a Pesquisa da Microsoft aos seus aplicativos. Consulte dados que a Pesquisa da Microsoft indexa e inclua dados externos personalizados.
ms.localizationpriority: high
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: ee2a62e6be739122140ccadefd993e069fa9e6cd
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446088"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Visão geral da API da Pesquisa da Microsoft no Microsoft Graph

A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização. Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados. A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing. Você pode usar a API de pesquisa da Microsoft no Microsoft Graph para estender a pesquisa da Microsoft para seus aplicativos.

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Por que usar a API de Pesquisa da Microsoft?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft

A API de pesquisa da Microsoft fornece um ponto de extremidade de pesquisa unificado que você pode usar para [consultar](/graph/api/search-query) dados nas mensagens e eventos na nuvem da Microsoft&mdash; em caixas de correio e arquivos do Outlook no OneDrive e no SharePoint&mdash; que a Pesquisa da Microsoft já indexa.

### <a name="include-custom-external-data-in-search-experience"></a>Incluir dados externos personalizados na experiência de pesquisa

Use os [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) para incluir dados que estejam fora da nuvem da Microsoft em sua experiência de pesquisa. Por exemplo, conecte-se ao banco de dados de recursos humanos ou ao catálogo de produtos da organização. Em seguida, use a API de Pesquisa da Microsoft para [consultar](/graph/api/search-query) diretamente a fonte de dados externa.

Navegue na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) para encontrar conectores prontos para uso. Alternativamente, você pode [construir seus próprios conectores](/graph/api/resources/indexing-api-overview#common-use-cases) para indexar itens personalizados externos e consultar fontes de dados externas específicas.

### <a name="consistent-up-to-date-search-experience"></a>Experiência de pesquisa atualizada e consistente

Ao usar a API de pesquisa da Microsoft, seus clientes se beneficiam dos resultados de pesquisa relevantes mais personalizados com a plataforma Microsoft Graph. A experiência de pesquisa em seus aplicativos retorna resultados que são consistentes com a pesquisa em aplicativos do Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Quais dados posso adicionar ou acessar usando a API de pesquisa da Microsoft?

A API de pesquisa da Microsoft suporta para pesquisar o seguinte conteúdo na nuvem da Microsoft: 

- Recursos de [mensagens](/graph/api/resources/message) de email e [eventos](/graph/api/resources/event) do calendário do Outlook.
- Arquivos e pastas do SharePoint e OneDrive (recursos [driveItem](/graph/api/resources/driveitem)), [lista](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) e recursos de [unidade](/graph/api/resources/drive).
- Recursos [pessoais](/graph/api/resources/person) em uma organização que são mais relevantes para um usuário.
- Conteúdo ingerido por meio da plataforma de conectores do Microsoft Graph: recursos [externalItem](/graph/api/resources/externalitem).
- Recursos de resposta de pesquisa administrativa: [acrônimos](/graph/api/resources/search-acronym), [indicadores](/graph/api/resources/search-bookmark) e [recursos QnA](/graph/api/resources/search-qna).

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [Usar a API de Pesquisa da Microsoft para consultar dados v1.0](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)
- [Usar a API de Pesquisa da Microsoft para consultar dados beta](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [Usar a API de Pesquisa da Microsoft para indexar dados](/graph/api/resources/indexing-api-overview)
- [Usar a API de Pesquisa da Microsoft para gerenciar as respostas de pesquisa administrativa beta](/graph/api/resources/search-api-answers-overview?view=graph-rest-beta&preserve-view=true) (versão prévia)

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).
- Saiba mais sobre alguns dos principais casos de uso:
  - [Gerenciar conexões para indexar conteúdo externo](connecting-external-content-manage-connections.md)
  - [Indexar conteúdo externo](connecting-external-content-manage-items.md)
  - [Pesquisar mensagens do Outlook](search-concept-messages.md)
  - [Pesquisar eventos do calendário](search-concept-events.md)
  - [Pesquisar conteúdo no OneDrive e Microsoft Office SharePoint Online](search-concept-files.md)
  - [Pesquisar conteúdo externo](search-concept-custom-types.md)
  - [Pesquisar pessoa](search-concept-person.md) (visualização)
  - [Gerenciar respostas de pesquisa administrativa](search-concept-answers.md) (versão prévia)
  - [Gerenciar o layout dos resultados de pesquisa](search-concept-display-layout.md) (versão prévia)
  - [Refinar resultados de pesquisa](search-concept-aggregation.md)
  - [Solicitar correção ortográfica](search-concept-speller.md) (versão prévia)
  - [Classificar resultados de pesquisa](search-concept-sort.md)
  - [Usar modelos de consulta](search-concept-query-template.md) (versão prévia)
  - [Resultados duplicados da pesquisa](search-concept-trim-duplicate.md) (versão prévia)
- Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.
- Interaja com a comunidade do [Microsoft Q&A](/answers/products/m365#microsoft-graph) ou no GitHub.
