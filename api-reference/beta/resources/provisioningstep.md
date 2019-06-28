---
title: tipo de recurso provisioningStep
description: 'Descreve as etapas executadas para executar uma ação. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349317"
---
# <a name="provisioningstep-resource-type"></a>tipo de recurso provisioningStep

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve as etapas executadas para executar uma ação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Resumo do que ocorreu durante a etapa.|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes sobre o que ocorreu durante a etapa.|
|name|Cadeia de caracteres|Nome da etapa.|
|provisioningStepType|String| Tipo de etapa. Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|String| Status da etapa. Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
