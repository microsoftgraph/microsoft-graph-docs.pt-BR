---
title: Tipo de recurso recommendLabelAction
description: Representa um rótulo que deve ser recomendado ao usuário para o aplicativo para o arquivo com base em tipos de informações confidenciais.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 245aae5c65d08d5a1755434917afe9b22f4c43b2
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883835"
---
# <a name="recommendlabelaction-resource-type"></a>Tipo de recurso recommendLabelAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um rótulo que deve ser recomendado para o usuário para o aplicativo para o arquivo com base em tipos de informações confidenciais descobertas. [EvaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) poderá retornar uma **recommendLabelAction** se a política de rotulagem da Proteção de Informações do Microsoft Purview  estiver definida para recomendar e rotular, em vez de impor um rótulo. O usuário ou a agregação pode optar por ignorar ou aceitar a recomendação. 

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                                     | Descrição                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| actionSource                | String                                                                   | Os valores possíveis são: `manual`, `automatic`, `recommended`, `default`. |
| actions                     | [coleção informationProtectionAction](informationprotectionaction.md) | Ações a serem tomadas se o rótulo for aceito pelo usuário.                                                                       |
| rótulo                       | [labelDetails](labeldetails.md)                                          | O rótulo que está sendo recomendado.                                                                      |
| responsibleSensitiveTypeIds | Coleção de GUIDs                                                          | Os GUIDs de tipo de informações confidenciais que causaram a recomendação.                                                                      |

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


