---
title: Tipo de recurso provisioningStep
description: 'Descreve as etapas tomadas para executar uma ação. '
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ea8b16437277c363a8e691c893d046301c3eead4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078705"
---
# <a name="provisioningstep-resource-type"></a>Tipo de recurso provisioningStep

Namespace: microsoft.graph

Descreve as etapas tomadas para executar uma ação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Resumo do que ocorreu durante a etapa.|
|detalhes|[detailsInfo](detailsinfo.md)|Detalhes do que ocorreu durante a etapa.|
|nome|Cadeia de caracteres|Nome da etapa.|
|provisioningStepType|provisioningStepType| Tipo de etapa. Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|provisioningResult| Status da etapa. Os valores possíveis são: `success` , , , , `warning`  `failure` `skipped` `unknownFutureValue` .|

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


