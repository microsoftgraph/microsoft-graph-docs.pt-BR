---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4b350c5ebe39da336dfe467bb73f5b91270dc31c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345794"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="8aa75-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8aa75-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa75-104">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="8aa75-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8aa75-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8aa75-105">Properties</span></span>

| <span data-ttu-id="8aa75-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aa75-106">Property</span></span>            | <span data-ttu-id="8aa75-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aa75-107">Type</span></span>     | <span data-ttu-id="8aa75-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aa75-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8aa75-109">id</span><span class="sxs-lookup"><span data-stu-id="8aa75-109">id</span></span>                  | <span data-ttu-id="8aa75-110">string</span><span class="sxs-lookup"><span data-stu-id="8aa75-110">string</span></span>   | <span data-ttu-id="8aa75-111">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="8aa75-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="8aa75-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="8aa75-112">teamsAppId</span></span>          | <span data-ttu-id="8aa75-113">string</span><span class="sxs-lookup"><span data-stu-id="8aa75-113">string</span></span>   | <span data-ttu-id="8aa75-114">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="8aa75-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="8aa75-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8aa75-115">displayName</span></span>         | <span data-ttu-id="8aa75-116">string</span><span class="sxs-lookup"><span data-stu-id="8aa75-116">string</span></span>   | <span data-ttu-id="8aa75-117">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8aa75-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="8aa75-118">versão</span><span class="sxs-lookup"><span data-stu-id="8aa75-118">version</span></span>             | <span data-ttu-id="8aa75-119">string</span><span class="sxs-lookup"><span data-stu-id="8aa75-119">string</span></span>   | <span data-ttu-id="8aa75-120">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8aa75-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8aa75-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8aa75-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="8aa75-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="8aa75-122">See also</span></span>

- [<span data-ttu-id="8aa75-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8aa75-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="8aa75-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8aa75-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8aa75-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8aa75-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

