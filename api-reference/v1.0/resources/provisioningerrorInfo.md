---
title: provisionamentoErrorInfo tipo de recurso
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a682e176b40d58e2dc0a794b58b8561f8948d5a5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547152"
---
# <a name="provisioningerrorinfo-resource-type"></a>provisionamentoErrorInfo tipo de recurso

Namespace: microsoft.graph


Descreve o status do evento de provisionamento e os erros associados. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|additionalDetails|Cadeia de caracteres|Detalhes adicionais em caso de erro.|
|erroCategoria|provisionamentoStatusErrorCategory|Categoriza o código de erro. Os valores possíveis `failure` `nonServiceFailure` são, `success` , , `unknownFutureValue`|
|errorCode|Cadeia de caracteres|Código de erro único, se ocorreu algum. [Saiba mais](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|motivo|Cadeia de caracteres|Resume o status e descreve por que o status aconteceu.|
|recomendaçãoAction|Cadeia de caracteres|Fornece a resolução para o erro correspondente.|

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


