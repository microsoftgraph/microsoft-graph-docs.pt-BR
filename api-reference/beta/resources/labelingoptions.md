---
title: tipo de recurso labelingOptions
description: Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8883c08bbd1f351dc5de003988f36c727ef85d7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939296"
---
# <a name="labelingoptions-resource-type"></a>tipo de recurso labelingOptions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as opções de rótulo que podem ser fornecidas para as APIs de avaliação. **labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo que deve ser aplicado. 

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo                                                | Descrição                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| AssignmentMethod for utilizado       | String                                              | Os valores possíveis são: `standard`, `privileged`, `auto`.                                                                        |
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