---
title: tipo de recurso teamDiscoverySettings
description: Configurações para configurar a descoberta de equipe por outras pessoas.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 56284b678dec74e00724eeb429958aa54444208d
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818697"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="7e7f9-103">tipo de recurso teamDiscoverySettings</span><span class="sxs-lookup"><span data-stu-id="7e7f9-103">teamDiscoverySettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e7f9-104">Fornece configurações para permitir que outras pessoas configurem a descoberta da [equipe](team.md) .</span><span class="sxs-lookup"><span data-stu-id="7e7f9-104">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="7e7f9-105">Você só pode modificar as configurações de descoberta para equipes privadas.</span><span class="sxs-lookup"><span data-stu-id="7e7f9-105">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="7e7f9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e7f9-106">Properties</span></span>
| <span data-ttu-id="7e7f9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e7f9-107">Property</span></span>     | <span data-ttu-id="7e7f9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e7f9-108">Type</span></span>   |<span data-ttu-id="7e7f9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e7f9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e7f9-110">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="7e7f9-110">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="7e7f9-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e7f9-111">Boolean</span></span>|<span data-ttu-id="7e7f9-112">Se for definido como true, a equipe ficará visível via pesquisa e sugestões do cliente do teams.</span><span class="sxs-lookup"><span data-stu-id="7e7f9-112">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e7f9-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e7f9-113">JSON representation</span></span>

<span data-ttu-id="7e7f9-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e7f9-114">The following is a JSON representation of the resource.</span></span>

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
