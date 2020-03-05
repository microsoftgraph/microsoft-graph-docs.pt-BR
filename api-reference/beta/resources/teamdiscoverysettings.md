---
title: tipo de recurso teamDiscoverySettings
description: Configurações de capacidade de descoberta da equipe por outras pessoas.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9a668c9d3b234fede0ad5c151e1dbbc95fc93516
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519957"
---
# <a name="teamdiscoverysettings-resource-type"></a>tipo de recurso teamDiscoverySettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações para permitir que outras pessoas configurem a descoberta da [equipe](team.md) . Você só pode modificar as configurações de descoberta para equipes privadas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|showInTeamsSearchAndSuggestions|Boolean|Se for definido como true, a equipe ficará visível via pesquisa e sugestões do cliente do teams.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDiscoverySettings"
}-->

```json
{
  "showInTeamsSearchAndSuggestions": true
}
```

<!-- uuid: f1d42106-0b3d-4930-9f19-d76f4e03b36b
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's discoverySettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamdiscoverysettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
