---
title: Tipo de recurso recommendLabelAction
description: Representa um rótulo que deve ser recomendado ao usuário para aplicativo para o arquivo com base em tipos de informações confidenciais.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 10d3ac687605ab648cdd3d68d6a3721c8fba2e30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962568"
---
# <a name="recommendlabelaction-resource-type"></a>Tipo de recurso recommendLabelAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um rótulo que deve ser recomendado ao usuário para o aplicativo para o arquivo com base em tipos de informações confidenciais descobertos. A [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) poderá retornar uma **recommendLabelAction** se a política  de rotulagem da Proteção de Informações da Microsoft estiver definida como recomendar e rotular, em vez de impor um rótulo. O usuário ou a aplicação pode optar por ignorar ou aceitar a recomendação. 

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                                     | Descrição                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| actionSource                | String                                                                   | Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`. |
| actions                     | [Coleção informationProtectionAction](informationprotectionaction.md) | Ações a ser tomadas se o rótulo for aceito pelo usuário.                                                                       |
| rótulo                       | [labelDetails](labeldetails.md)                                          | O rótulo que está sendo recomendado.                                                                      |
| responsibleSensitiveTypeIds | Coleção de GUIDs                                                          | Os GUIDs do tipo de informação confidenciais que causaram a recomendação a ser dada.                                                                      |

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


