---
title: Tipo de recurso provisioningErrorInfo
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: de8804ab2ae1e1e8f9516e25c0f0a5522d86a0ff2c3722fb9c10e47bc575869c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205195"
---
# <a name="provisioningerrorinfo-resource-type"></a>Tipo de recurso provisioningErrorInfo

Namespace: microsoft.graph


Descreve o status do evento de provisionamento e os erros associados. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|additionalDetails|Cadeia de caracteres|Detalhes adicionais em caso de erro.|
|errorCategory|provisioningStatusErrorCategory|Categoriza o código de erro. Os valores possíveis `failure` são `nonServiceFailure` , , `success` , `unknownFutureValue`|
|errorCode|Cadeia de caracteres|Código de erro exclusivo se ocorrer algum. [Saiba Mais](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|motivo|Cadeia de caracteres|Resume o status e descreve por que o status aconteceu.|
|recommendedAction|Cadeia de caracteres|Fornece a resolução do erro correspondente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningErrorInfo",
  "baseType": null
}-->

```json
{
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
  "description": "provisioningErrorInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


