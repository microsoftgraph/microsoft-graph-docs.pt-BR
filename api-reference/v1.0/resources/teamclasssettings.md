---
title: tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo classe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 40b1e21933adedaf8d1c4e16aa91d69c4af17668
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094040"
---
# <a name="teamclasssettings-resource-type"></a>tipo de recurso teamClassSettings

Namespace: microsoft.graph

Representa propriedades específicas de classe de uma [equipe](team.md). Disponível apenas quando a equipe representa uma classe.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Booliano|Se for definido como `true` , habilitará o envio de emails de Resumo de atribuições semanais para pais/guardiões, desde que a administração de locatários tenha habilitado a configuração globalmente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

