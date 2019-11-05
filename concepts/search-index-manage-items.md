---
title: Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft
description: Aprenda a usar o Microsoft Graph para gerenciar itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 522566fb59771dc9a4efab305a271dc89a4843af
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939520"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a>Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft

Os itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft são representados pelos recursos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) e [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) no Microsoft Graph.

O recurso **externalItem** representa um tipo personalizado. Ele deve ser usado quando os itens que você adiciona ao índice usam um esquema personalizado não representado pelo recurso **externalFile**. Por exemplo, tíquetes de assistência técnica ou lista de produtos.

O recurso **externalFile** representa um arquivo em um sistema externo.

> [!NOTE]
> O esquema para **externalFile** não pode ser estendido.

## <a name="add-an-item-or-file"></a>Adicionar um item ou arquivo

Você pode adicionar um item ou arquivo ao índice [criando um externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta). Ao criar um item, você atribui um identificador exclusivo na URL.

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

## <a name="update-an-item-or-file"></a>Atualizar um item ou arquivo

Quando um item ou arquivo é atualizado no serviço externo (o tíquete da assistência técnica é reatribuído ou a descrição do produto é atualizada), você pode atualizar sua entrada no índice [atualizando o externalItem](/graph/api/externalitem-update?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando você o criou.

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item-or-file"></a>Excluir um item ou arquivo

Você pode remover itens ou arquivos do índice [excluindo o externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando você o criou.

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>Próximas etapas

- [Por que usar a API de Pesquisa da Microsoft?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Usar a API de Pesquisa da Microsoft para indexar dados](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Pesquisar tipos personalizados (externalItem)](search-concept-custom-types.md)
- [Pesquisar arquivos (incluindo externalFile)](search-concept-files.md)
- Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub
