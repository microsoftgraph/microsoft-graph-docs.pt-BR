---
title: tipo de recurso labelingOptions
description: Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: da2231ae3eb95260663d2907f56f91b96e08278c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084013"
---
# <a name="labelingoptions-resource-type"></a>tipo de recurso labelingOptions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação. **labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo que deve ser aplicado. 

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo                                                | Descrição                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| AssignmentMethod for utilizado       | Cadeia de caracteres                                              | Os valores possíveis são: `standard`, `privileged`, `auto`.                                                                        |
| downgradeJustification | [downgradeJustification](downgradejustification.md) | O objeto Justification de downgrade que indica se o downgrade foi justificado e, em caso afirmativo, o motivo.                          |
| extendedProperties     | Coleção [keyValuePair](keyvaluepair.md)          | As propriedades estendidas serão analisadas e retornadas no formato de metadados MIP rotulado padrão como parte das informações do rótulo. |
| labelID                | Guid                                                | O GUID do rótulo que deve ser aplicado à informação.                                                              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelingOptions",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "downgradeJustification": {"@odata.type": "microsoft.graph.downgradeJustification"},
  "extendedProperties": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "labelId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelingOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

