---
title: tipo de recurso applyLabelAction
description: Representa um conjunto de ações que devem ser seguidas para aplicar ou atualizar um rótulo.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fc7911b3a225f226edc74dc9b194a2522b7c4251
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939142"
---
# <a name="applylabelaction-resource-type"></a>tipo de recurso applyLabelAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de ações que devem ser seguidas para aplicar ou atualizar um rótulo. **applyLabelAction** é retornado quando o resultado de uma operação de avaliação de rótulo é que um rótulo deve ser aplicado. A `actions` propriedade contém uma coleção [informationProtectionAction](informationProtectionaction.md) que descreveu o conjunto completo de ações para *aplicar* o rótulo, incluindo remoção de metadados antigos, marcação de conteúdo e proteção.

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                                     | Descrição                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ação                | String                                                                   | Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.                                                                                                                             |
| actions                     | coleção [informationProtectionAction](informationprotectionaction.md) | A coleção de ações específicas que devem ser tomadas pelo aplicativo de consumo para rotular o documento. Consulte [informationProtectionAction](informationprotectionaction.md) para obter a lista completa. |
| rótulo                       | [labelDetails](labeldetails.md)                                          | Objeto que descreve os detalhes do rótulo a ser aplicado.                                                                                                                                          |
| responsibleSensitiveTypeIds | Coleção de GUIDs                                                          | Se o rótulo foi o resultado de uma classificação automática, forneça a lista de GUIDs de tipo de informações confidenciais que resultaram no rótulo retornado.                                         
## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applyLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applyLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->