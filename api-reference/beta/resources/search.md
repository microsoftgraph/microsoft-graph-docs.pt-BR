---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bb38d281895ac11d97a026a4352f68b93e8ba801
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704059"
---
# <a name="search-resource-type"></a>tipo de recurso de pesquisa

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa. Ele serve como uma âncora para a ação de [consulta](../api/search-query.md) .

Esse recurso não deve ser chamado como tal. Qualquer solicitação no recurso causará uma solicitação incorreta.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a>Representação JSON

Nenhum

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

Nenhum

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [query](../api/search-query.md) | [searchResponse](searchresponse.md) Coletânea| Executa a consulta especificada no [searchRequest](../resources/searchrequest.md) |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
