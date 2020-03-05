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
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="a37f2-103">tipo de recurso teamDiscoverySettings</span><span class="sxs-lookup"><span data-stu-id="a37f2-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="a37f2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a37f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a37f2-105">Fornece configurações para permitir que outras pessoas configurem a descoberta da [equipe](team.md) .</span><span class="sxs-lookup"><span data-stu-id="a37f2-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="a37f2-106">Você só pode modificar as configurações de descoberta para equipes privadas.</span><span class="sxs-lookup"><span data-stu-id="a37f2-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="a37f2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a37f2-107">Properties</span></span>
| <span data-ttu-id="a37f2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a37f2-108">Property</span></span>     | <span data-ttu-id="a37f2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a37f2-109">Type</span></span>   |<span data-ttu-id="a37f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a37f2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a37f2-111">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="a37f2-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="a37f2-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a37f2-112">Boolean</span></span>|<span data-ttu-id="a37f2-113">Se for definido como true, a equipe ficará visível via pesquisa e sugestões do cliente do teams.</span><span class="sxs-lookup"><span data-stu-id="a37f2-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a37f2-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a37f2-114">JSON representation</span></span>

<span data-ttu-id="a37f2-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a37f2-115">The following is a JSON representation of the resource.</span></span>

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
