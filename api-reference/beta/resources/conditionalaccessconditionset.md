---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dee80ebdacfda6c0b633f1aec1dd085d80eb22e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507559"
---
# <a name="conditionalaccessconditionset-resource-type"></a>tipo de recurso conditionalAccessConditionSet

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tipo de condições que controlam quando a política se aplica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Emprego|[conditionalAccessApplications](conditionalaccessapplications.md)| Aplicativos e ações do usuário incluídos no e excluídos da política. Obrigatório. |
|usuários|[conditionalAccessUsers](conditionalaccessusers.md)| Usuários, grupos e funções incluídos no e excluídos da política. Obrigatório. |
|clientAppTypes|String collection| Tipos de aplicativo cliente incluídos na política. Os valores possíveis são: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| Estados do dispositivo na política. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Locais incluídos no e excluídos da política. |
|plataformas|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Plataformas incluídas e excluídas da política. |
|signInRiskLevels|String collection| Níveis de risco incluídos na política. Os valores possíveis são: `low`, `medium`, `high`, `none`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->