---
title: tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo classe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8d345cd229c4a6c003c87865b5aaddf01096b4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998613"
---
# <a name="teamclasssettings-resource-type"></a>tipo de recurso teamClassSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa propriedades específicas de classe de uma [equipe](team.md). Disponível somente quando a equipe representa uma classe.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Booliano|Se for definido `true`como, habilitará o envio de emails de Resumo de atribuições semanais para pais/guardiões, desde que a administração de locatários tenha habilitado a configuração globalmente.|

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
