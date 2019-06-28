---
title: tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d3c22e67af690a28bb974a0334af7891f0c25cfb
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349325"
---
# <a name="statusdetails-resource-type"></a>tipo de recurso statusDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status do evento de provisionamento e os erros associados. Ela é herdada de [statusBase](/graph/api/resources/statusBase?view=graph-rest-beta) e usada apenas quando status é definido como ' Failure '.  

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|String|Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`. Herdado de statusBase.|
|additionalDetails|String|Detalhes adicionais em caso de erro.|
|errorCategory|String|Categoriza o código de erro.|
|errorCode|Cadeia de caracteres|Código de erro exclusivo, caso algum tenha ocorrido.|
|motivos|String|Resume o status e descreve por que o status ocorreu.|
|recomendado|String|Fornece a resolução para o erro correspondente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
