---
title: Tipo de recurso provisioningErrorInfo
description: Descreve o status do evento de provisionamento e os erros associados.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f0b6e42fc184db1d8c2044d56820d0e19e89f8c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019164"
---
# <a name="provisioningerrorinfo-resource-type"></a>Tipo de recurso provisioningErrorInfo

Namespace: microsoft.graph


Descreve o status do evento de provisionamento e os erros associados. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|additionalDetails|String|Detalhes adicionais em caso de erro.|
|errorCategory|provisioningStatusErrorCategory|Categoriza o código de erro. Os valores possíveis `failure` são `nonServiceFailure` , , `success` , `unknownFutureValue`|
|errorCode|Cadeia de caracteres|Código de erro exclusivo se ocorrer algum. [Saiba mais](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
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


