---
title: tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 853f7ba95ca4e569efd57bb46024b4258b098d90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520314"
---
# <a name="statusdetails-resource-type"></a>tipo de recurso statusDetails

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status do evento de provisionamento e os erros associados. Ela é herdada de [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) e usada apenas quando status é definido como ' Failure '.  

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|String|Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`. Herdado de statusBase.|
|additionalDetails|String|Detalhes adicionais em caso de erro.|
|errorCategory|String|Categoriza o código de erro.|
|errorCode|Cadeia de caracteres|Código de erro exclusivo, caso algum tenha ocorrido.|
|motivo|String|Resume o status e descreve por que o status ocorreu.|
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
