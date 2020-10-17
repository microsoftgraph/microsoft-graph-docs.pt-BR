---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 431ea73f20b36b189ae7638cc56a01239c1f113f
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582125"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>tipo de recurso conditionalAccessGrantControls

Namespace: microsoft.graph

Representa os controles de concessão que devem ser atendidos para passar a política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| operator | String | Define o relacionamento dos controles de concessão. Valores possíveis: `AND` , `OR` . |
| builtInControls | String collection | Lista de valores de controles internos exigidos pela política. Valores possíveis: `Block` , `Mfa` ,,, `CompliantDevice` `DomainJoinedDevice` `ApprovedApplication` , `CompliantApplication` |
| customAuthenticationFactors | String collection | Lista de IDs de controles personalizados exigidos pela política. Para obter mais informações, consulte [Custom Controls](/azure/active-directory/conditional-access/controls). |
| termsOfUse | String collection | Lista de [termos de uso](/graph/api/resources/agreement) IDs exigidos pela política. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->