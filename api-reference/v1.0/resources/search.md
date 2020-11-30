---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8e9d8bc133a050701543f2a978e56b662bafcc33
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377962"
---
# <a name="search-resource-type"></a>tipo de recurso de pesquisa

Namespace: microsoft.graph

O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa. Ele serve como uma âncora para a ação de [consulta](../api/search-query.md) .

Esse recurso não deve ser chamado como tal. Qualquer solicitação no recurso causará uma solicitação incorreta.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a>Representação JSON

Nenhum

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

Nenhuma

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


