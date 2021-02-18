---
title: Tipo de recurso teamDiscoverySettings
description: Configurações de capacidade de descoberta da equipe por outras pessoas.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: edc3c6cc446e35f2f5a97212d3c0b6f69b81ce30
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292880"
---
# <a name="teamdiscoverysettings-resource-type"></a>Tipo de recurso teamDiscoverySettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações para permitir que outras pessoas configurem a [capacidade de descoberta](team.md) da equipe. Você só pode modificar as configurações de descoberta para equipes privadas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|showInTeamsSearchAndSuggestions|Booliano|Se definido como verdadeiro, a equipe é visível por meio de pesquisa e sugestões do cliente do Teams.|

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
  ]
}-->


