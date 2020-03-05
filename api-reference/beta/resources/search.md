---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8cb963c0fda545ea88e8d8e4335954ffb455102f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520932"
---
# <a name="search-resource-type"></a>tipo de recurso de pesquisa

Namespace: Microsoft. Graph

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
