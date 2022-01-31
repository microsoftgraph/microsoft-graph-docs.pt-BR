---
title: tipo de recurso de pesquisa
description: O objeto de nível superior que representa o ponto de extremidade de pesquisa no Microsoft Graph.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 034e1adec8d1bcee0336abdbeed2d980ee559964
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282028"
---
# <a name="search-resource-type"></a>tipo de recurso de pesquisa

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O objeto de nível superior que representa o ponto de extremidade de pesquisa. Ele serve como uma âncora para a [ação de](../api/search-query.md) consulta.

Esse recurso não é chamado. Qualquer solicitação que chamar esse recurso resultará em uma resposta HTTP `400 Bad Request` .

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [query](../api/search-query.md) | [Coleção searchResponse](searchresponse.md)| Execute uma consulta de pesquisa especificada. |

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Nenhum

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


