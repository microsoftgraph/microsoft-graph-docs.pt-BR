---
title: Tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d817c0aa46dde6b49debd849d8fd2ae61e06a672
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956814"
---
# <a name="statusdetails-resource-type"></a>Tipo de recurso statusDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status do evento de provisionamento e os erros associados. Ele é herdado do [statusBase](/graph/api/resources/statusbase) e usado somente quando o status é definido como `failure` .  

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|statusBase|Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`. Herdado do statusBase.|
|additionalDetails|Cadeia de caracteres|Detalhes adicionais em caso de erro.|
|errorCategory|Cadeia de caracteres|Categoriza o código de erro. Os valores possíveis são `Failure`, `NonServiceFailure`, `Success`.|
|errorCode|Cadeia de caracteres|Código de erro exclusivo se ocorrer algum. [Saiba Mais](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|motivo|Cadeia de caracteres|Resume o status e descreve por que o status aconteceu.|
|recommendedAction|Cadeia de caracteres|Fornece a resolução do erro correspondente.|

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


