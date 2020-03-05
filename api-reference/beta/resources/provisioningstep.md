---
title: tipo de recurso provisioningStep
description: 'Descreve as etapas executadas para executar uma ação. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4275730cfd7c9c9c58496b674062ffedb5d7a6cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521324"
---
# <a name="provisioningstep-resource-type"></a>tipo de recurso provisioningStep

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve as etapas executadas para executar uma ação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Resumo do que ocorreu durante a etapa.|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes sobre o que ocorreu durante a etapa.|
|nome|Cadeia de caracteres|Nome da etapa.|
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
