---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b91afb44cc43c3c6ac4970afc36914abcb08c4c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507545"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>tipo de recurso conditionalAccessGrantControls

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os controles de concessão que devem ser atendidos para passar a política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| operator | String | Define o relacionamento dos controles de concessão. Valores possíveis: `AND`, `OR`. |
| builtInControls | String collection | Lista de valores de controles internos exigidos pela política. Valores possíveis: `Block`, `Mfa`, `CompliantDevice` `DomainJoinedDevice`,, `ApprovedApplication`,`CompliantApplication` |
| customAuthenticationFactors | String collection | Lista de IDs de controles personalizados exigidos pela política. Saiba mais sobre os controles personalizados aqui:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview |
| termsOfUse | String collection | Lista de [termos de uso](agreement.md) IDs exigidos pela política. |

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