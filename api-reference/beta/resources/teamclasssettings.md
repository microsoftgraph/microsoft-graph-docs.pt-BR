---
title: tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo classe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 50fd73203697b008163337eb32ab9b54c0e8fd0b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519964"
---
# <a name="teamclasssettings-resource-type"></a>tipo de recurso teamClassSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades específicas de classe de uma [equipe](team.md). Disponível apenas quando a equipe representa uma classe.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Boolean|Se for definido `true`como, habilitará o envio de emails de Resumo de atribuições semanais para pais/guardiões, desde que a administração de locatários tenha habilitado a configuração globalmente.|

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
