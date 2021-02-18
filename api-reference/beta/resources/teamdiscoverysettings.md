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
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="12b64-103">Tipo de recurso teamDiscoverySettings</span><span class="sxs-lookup"><span data-stu-id="12b64-103">teamDiscoverySettings resource type</span></span>

<span data-ttu-id="12b64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12b64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12b64-105">Fornece configurações para permitir que outras pessoas configurem a [capacidade de descoberta](team.md) da equipe.</span><span class="sxs-lookup"><span data-stu-id="12b64-105">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="12b64-106">Você só pode modificar as configurações de descoberta para equipes privadas.</span><span class="sxs-lookup"><span data-stu-id="12b64-106">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="12b64-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12b64-107">Properties</span></span>
| <span data-ttu-id="12b64-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12b64-108">Property</span></span>     | <span data-ttu-id="12b64-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12b64-109">Type</span></span>   |<span data-ttu-id="12b64-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12b64-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12b64-111">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="12b64-111">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="12b64-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="12b64-112">Boolean</span></span>|<span data-ttu-id="12b64-113">Se definido como verdadeiro, a equipe é visível por meio de pesquisa e sugestões do cliente do Teams.</span><span class="sxs-lookup"><span data-stu-id="12b64-113">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12b64-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12b64-114">JSON representation</span></span>

<span data-ttu-id="12b64-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12b64-115">The following is a JSON representation of the resource.</span></span>

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


