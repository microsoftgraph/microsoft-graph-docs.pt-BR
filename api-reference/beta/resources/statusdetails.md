---
title: Tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e3333ac030ec08722ad6bcaa58a153fc961469cf
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546901"
---
# <a name="statusdetails-resource-type-deprecated"></a>Tipo de recurso statusDetails (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> A API statusDetails está preterida e interromperá o retorno de dados em 31 de dezembro de 2021. Use o novo tipo [provisioningStatusInfo.](provisioningstatusinfo.md)

Descreve o status do evento de provisionamento e os erros associados. Ele é herdado do [statusBase](/graph/api/resources/statusbase) e usado somente quando o status é definido como `failure` .  

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|statusBase|Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`. Herdado do statusBase.|
|additionalDetails|String|Detalhes adicionais em caso de erro.|
|errorCategory|String|Categoriza o código de erro. Os valores possíveis são `Failure`, `NonServiceFailure`, `Success`.|
|errorCode|Cadeia de caracteres|Código de erro exclusivo se ocorrer algum. [Saiba mais](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|motivo|String|Resume o status e descreve por que o status aconteceu.|
|recommendedAction|String|Fornece a resolução do erro correspondente.|

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


