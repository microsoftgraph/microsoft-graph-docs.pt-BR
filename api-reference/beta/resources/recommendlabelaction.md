---
title: tipo de recurso recommendLabelAction
description: Representa um rótulo que deve ser recomendado para o usuário para o aplicativo para o arquivo com base em tipos de informações confidenciais.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f2a872c0aa64eb79e0b8755ddc6b3788f14055
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939373"
---
# <a name="recommendlabelaction-resource-type"></a>tipo de recurso recommendLabelAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um rótulo que deve ser recomendado para o usuário para o aplicativo no arquivo com base em tipos de informações confidenciais descobertos. O [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) poderá retornar um **recommendLabelAction** se a política de rótulo de proteção de informações da Microsoft estiver definida como **recomendar** e rotular em vez de impor um rótulo. O usuário ou a aplicação pode optar por ignorar ou aceitar a recomendação. 

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                                     | Descrição                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| ação                | String                                                                   | Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`. |
| actions                     | coleção [informationProtectionAction](informationprotectionaction.md) | Ações a serem executadas se o rótulo for aceito pelo usuário.                                                                       |
| rótulo                       | [labelDetails](labeldetails.md)                                          | O rótulo que está sendo recomendado.                                                                      |
| responsibleSensitiveTypeIds | Coleção de GUIDs                                                          | Os GUIDs de tipo de informações confidenciais que causaram a recomendação para serem fornecidos.                                                                      |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
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
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
