---
title: Tipo de recurso labelingOptions
description: Representa as opções de rotulagem que podem ser fornecidas às APIs de avaliação.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7d2409bf538de3d37ca32cdf2fd1afb78a659817
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950295"
---
# <a name="labelingoptions-resource-type"></a>Tipo de recurso labelingOptions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as opções de rotulagem que podem ser fornecidas às APIs de avaliação. **labelingOptions** deve ser passado para a API [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) para especificar detalhes sobre o rótulo a ser aplicado. 

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo                                                | Descrição                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| assignmentMethod       | Cadeia de caracteres                                              | Os valores possíveis são: `standard`, `privileged`, `auto`.                                                                        |
| downgradeJustification | [downgradeJustification](downgradejustification.md) | O objeto de justificativa de downgrade que indica se downgrade foi justificado e, em caso afirmado, o motivo.                          |
| extendedProperties     | Coleção [keyValuePair](keyvaluepair.md)          | As propriedades estendidas serão analisados e retornadas no formato de metadados padrão rotulados MIP como parte das informações do rótulo. |
| labelId                | Guid                                                | O GUID do rótulo que deve ser aplicado às informações.                                                              |

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

