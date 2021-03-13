---
title: Tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 61b0f11fcfb36c3773d196924e675d2e10871b63
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761013"
---
# <a name="statusdetails-resource-type"></a>Tipo de recurso statusDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status do evento de provisionamento e os erros associados. Ele é herdado do [statusBase](/graph/api/resources/statusbase) e usado somente quando o status é definido como `failure` .  

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|String|Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`. Herdado do statusBase.|
|additionalDetails|Cadeia de Caracteres|Detalhes adicionais em caso de erro.|
|errorCategory|Cadeia de Caracteres|Categoriza o código de erro. Os valores possíveis são `Failure`, `NonServiceFailure`, `Success`.|
|errorCode|Cadeia de caracteres|Código de erro exclusivo se ocorrer algum. [Saiba mais](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|motivo|Cadeia de Caracteres|Resume o status e descreve por que o status aconteceu.|
|recommendedAction|Cadeia de Caracteres|Fornece a resolução do erro correspondente.|

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


