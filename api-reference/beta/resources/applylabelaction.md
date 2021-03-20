---
title: Tipo de recurso applyLabelAction
description: Representa um conjunto de ações que devem ser tomadas para aplicar ou atualizar um rótulo.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e53a2796c7cd4f0b8c0a415ca4bc38ffefeb609e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945736"
---
# <a name="applylabelaction-resource-type"></a>Tipo de recurso applyLabelAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de ações que devem ser tomadas para aplicar ou atualizar um rótulo. **applyLabelAction** é retornado quando o resultado de uma operação de avaliação de rótulo é que um rótulo deve ser aplicado. A `actions` propriedade contém uma coleção [informationProtectionAction](informationProtectionaction.md) que  descreve o conjunto completo de ações para aplicar o rótulo, incluindo a remoção de metadados antigos, marcação de conteúdo e proteção.

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                                     | Descrição                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| actionSource                | String                                                                   | Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`.                                                                                                                             |
| actions                     | [Coleção informationProtectionAction](informationprotectionaction.md) | O conjunto de ações específicas que devem ser tomadas pelo aplicativo de consumo para rotular o documento. Consulte  [informationProtectionAction](informationprotectionaction.md) para obter a lista completa. |
| rótulo                       | [labelDetails](labeldetails.md)                                          | Objeto que descreve os detalhes do rótulo a ser aplicado.                                                                                                                                          |
| responsibleSensitiveTypeIds | Coleção de GUIDs                                                          | Se o rótulo foi o resultado de uma classificação automática, fornece a lista de GUIDs do tipo de informação confidenciais que resultaram no rótulo retornado.                                         
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

