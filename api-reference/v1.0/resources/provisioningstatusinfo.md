---
title: Tipo de recurso provisioningStatusInfo
description: Descreve o status do evento de resumo de provisionamento.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 82b13a700cece9b558ec131f68ea3f79fc0105c2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052871"
---
# <a name="provisioningstatusinfo-resource-type"></a>Tipo de recurso provisioningStatusInfo

Namespace: microsoft.graph


Descreve o status do evento de resumo de provisionamento. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|provisioningResult| Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.|
|errorInfo|[provisioningErrorInfo](provisioningErrorInfo.md)| Se o status não for bem-sucedido/ os detalhes ignorados do erro estão contidos nisso.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


