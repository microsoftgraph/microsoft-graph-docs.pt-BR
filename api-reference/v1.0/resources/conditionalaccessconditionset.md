---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3163bbefef420a878364f52f9dabc8dee1e7cae
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013671"
---
# <a name="conditionalaccessconditionset-resource-type"></a>Tipo de recurso conditionalAccessConditionSet

Namespace: microsoft.graph

Representa o tipo de condições que regem quando a política se aplica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applications|[conditionalAccessApplications](conditionalaccessapplications.md)| Aplicativos e ações do usuário incluídos e excluídos da política. Obrigatório. |
|usuários|[conditionalAccessUsers](conditionalaccessusers.md)| Usuários, grupos e funções incluídos e excluídos da política. Obrigatório. |
|clientAppTypes|Coleção String| Tipos de aplicativo cliente incluídos na política. Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.|
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Locais incluídos e excluídos da política. |
|platforms|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Plataformas incluídas e excluídas da política. |
|signInRiskLevels|Coleção String| Níveis de risco de login incluídos na política. Os valores possíveis são: `low`, `medium`, `high`, `none`.|
|userRiskLevels|Coleção String| Níveis de risco do usuário incluídos na política. Os valores possíveis são: `low`, `medium`, `high`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

