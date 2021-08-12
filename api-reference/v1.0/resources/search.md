---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f20a7d0513f084dadc8dc3f3693a7dd51109fb7e9ccbb163a80a17a29d6978f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251805"
---
# <a name="search-resource-type"></a>tipo de recurso de pesquisa

Namespace: microsoft.graph

O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa. Ele serve como uma âncora para a [ação de](../api/search-query.md) consulta.

Não é esperado que esse recurso seja chamado dessa forma. Qualquer solicitação no recurso incorre em uma Solicitação Inovada.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a>Representação JSON

None

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

Nenhuma

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [query](../api/search-query.md) | [searchResponse](searchresponse.md) Coleção| Executa a consulta especificada no [searchRequest](../resources/searchrequest.md) |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


