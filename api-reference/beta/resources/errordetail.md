---
title: tipo de recurso errorDetail
description: Descreve um erro para uma solicitação com falha para criar um esquema de conexão de pesquisa da Microsoft de forma assíncrona.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6f37f3ca432dcd9c755556b37f4f0ea330907426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013720"
---
# <a name="errordetail-resource-type"></a>tipo de recurso errorDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um erro para uma solicitação com falha para criar um [esquema](schema.md) de conexão de pesquisa da Microsoft de forma assíncrona.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo                                               | Descrição |
|:----------|:---------------------------------------------------|:------------|
| detalhes   | coleção [innerErrorDetail](innererrordetail.md) | Uma coleção de erros internos, se houver. Somente leitura, anulável. |
| errorCode | Cadeia de caracteres                                             | O código de erro associado ao erro, se houver. Somente leitura, anulável. |
| mensagem   | String                                             | A mensagem de erro legível por pessoas. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "details",
    "errorCode"
  ],
  "@odata.type": "microsoft.graph.errorDetail",
  "baseType": null
}-->

```json
{
  "details": [{"@odata.type": "microsoft.graph.innerErrorDetail"}],
  "errorCode": "String",
  "message": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "errorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


