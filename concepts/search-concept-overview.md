---
title: Visão geral da API da Pesquisa da Microsoft no Microsoft Graph
description: Use a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: eadfbc21f3f32fa15953a1a9979b04238191a8627ae48c2f6480dbd398a0e515
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211686"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Visão geral da API da Pesquisa da Microsoft no Microsoft Graph

A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização. Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados. A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing. Você pode usar a API de pesquisa da Microsoft no Microsoft Graph para estender a pesquisa da Microsoft para seus aplicativos.

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Por que usar a API de Pesquisa da Microsoft?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft

A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa que você pode usar para permitir que os desenvolvedores [consultem](/graph/api/search-query) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.

### <a name="include-custom-external-data-in-search-experience-preview"></a>Incluir dados externos personalizados na experiência de pesquisa (visualização)

Use[conectores do Microsoft Graph](/microsoftsearch/connectors-overview) para incluir dados de fora da nuvem da Microsoft em sua experiência de busca. Por exemplo, estabeleça uma conexão com o banco de dados de recursos humanos ou com o catálogo de produtos de uma organização. Em seguida, utilize a API de Pesquisa da Microsoft para [consultar](/graph/api/search-query) perfeitamente a fonte de dados externa. 

Navegue na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) para encontrar conectores prontos para uso. Alternativamente, você pode [construir seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) para indexar itens personalizados externos e consultar fontes de dados externas específicas.

### <a name="consistent-up-to-date-search-experience"></a>Experiência de pesquisa atualizada e consistente

Ao usar a API de pesquisa da Microsoft, seus clientes se beneficiam dos resultados de pesquisa relevantes mais personalizados com a plataforma Microsoft Graph. A experiência de pesquisa em seus aplicativos retorna resultados que são consistentes com a pesquisa em aplicativos do Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Quais dados posso adicionar ou acessar usando a API de pesquisa da Microsoft?

A API de pesquisa da Microsoft suporta para pesquisar o seguinte conteúdo na nuvem da Microsoft: 

- Recursos de [mensagens](/graph/api/resources/message) de email e [eventos](/graph/api/resources/event) do calendário do Outlook.
- Arquivos e pastas do SharePoint e OneDrive (recursos [driveItem](/graph/api/resources/driveitem)), [lista](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) e recursos de [unidade](/graph/api/resources/drive).
- Recursos [pessoais](/graph/api/resources/person) em uma organização que são mais relevantes para um usuário.
- Conteúdo ingerido por meio da plataforma de conectores do Microsoft Graph: recursos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true).

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)(v1.0)
- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)(pré-visualização)
- [Usar a API de Pesquisa da Microsoft para indexar dados](/graph/api/resources/indexing-api-overview) (pré-visualização)

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
  - [Classificar resultados de pesquisa](search-concept-sort.md) (pré-visualização)
  - [Refinar resultados de pesquisa](search-concept-aggregation.md) (pré-visualização)
  - [Solicitar correção ortográfica](search-concept-speller.md) (versão prévia)
  - [Layout de exibição de pesquisa](search-concept-display-layout.md) (versão prévia)
 
  
- Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.

## <a name="see-also"></a>Confira também

- Envolva-se com a comunidade no [Microsoft Q&A](/answers/products/m365#microsoft-graph)  ou no GitHub
