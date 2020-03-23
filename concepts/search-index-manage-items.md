---
title: Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft
description: Aprenda a usar o Microsoft Graph para gerenciar itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 5b969bd058b8c1e2790b0039a4369623287f641d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892783"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a>Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft

Os itens adicionados por seu aplicativo ao serviço de Pesquisa da Microsoft são representados pelo recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) no Microsoft Graph.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="add-an-item"></a>Adicionar um item

Você pode adicionar um item ao índice [criando um externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta). Ao criar um item, você atribui um identificador exclusivo na URL.

Por exemplo, seu aplicativo pode indexar tíquetes de assistência técnica usando o número do tíquete. Se um tíquete tiver o número do tíquete `SR00145`, a solicitação poderá ser semelhante à seguinte.

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> ![OBSERVAÇÃO] Antes que os itens indexados possam ser encontrados na IU da Pesquisa da Microsoft, um administrador deve [personalizar a página de resultados de pesquisa](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) para a conexão correspondente.

## <a name="update-an-item"></a>Atualizar um item

Quando um item é atualizado no serviço externo (o tíquete de assistência técnica é reatribuído ou uma descrição de produto é atualizada), você pode atualizar a respectiva entrada no índice [atualizando o externalItem](/graph/api/externalitem-update?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando ele foi criado.

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a>Excluir um item

Você pode remover os itens do índice [excluindo o externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando ele foi criado.

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>Próximas etapas

- [Por que usar a API de Pesquisa da Microsoft?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Ler a referência da API de Indexação](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Personalizar a página de resultados da pesquisa da Microsoft](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [Pesquisar tipos personalizados (externalItem)](search-concept-custom-types.md)
- Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub
