---
title: tipo de recurso errorDetail
description: Descreve um erro para uma solicitação com falha para criar um esquema de conexão de pesquisa da Microsoft de forma assíncrona.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7f77ccacd6e1f5339706549873ea4c75d9144e39
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704182"
---
# <a name="errordetail-resource-type"></a>tipo de recurso errorDetail

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
