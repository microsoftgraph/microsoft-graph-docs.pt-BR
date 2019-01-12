---
title: tipo de recurso de teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3aed533ecca3bff48071b04adadcea6b52169f89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951926"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="ed3b5-103">tipo de recurso de teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ed3b5-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="ed3b5-104">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed3b5-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ed3b5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed3b5-105">Properties</span></span>

| <span data-ttu-id="ed3b5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed3b5-106">Property</span></span>            | <span data-ttu-id="ed3b5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed3b5-107">Type</span></span>     | <span data-ttu-id="ed3b5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed3b5-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ed3b5-109">id</span><span class="sxs-lookup"><span data-stu-id="ed3b5-109">id</span></span>                  | <span data-ttu-id="ed3b5-110">string</span><span class="sxs-lookup"><span data-stu-id="ed3b5-110">string</span></span>   | <span data-ttu-id="ed3b5-111">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="ed3b5-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="ed3b5-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ed3b5-112">teamsAppId</span></span>          | <span data-ttu-id="ed3b5-113">string</span><span class="sxs-lookup"><span data-stu-id="ed3b5-113">string</span></span>   | <span data-ttu-id="ed3b5-114">A identificação de manifesto do aplicativo de equipes.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="ed3b5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ed3b5-115">displayName</span></span>         | <span data-ttu-id="ed3b5-116">string</span><span class="sxs-lookup"><span data-stu-id="ed3b5-116">string</span></span>   | <span data-ttu-id="ed3b5-117">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="ed3b5-118">version</span><span class="sxs-lookup"><span data-stu-id="ed3b5-118">version</span></span>             | <span data-ttu-id="ed3b5-119">string</span><span class="sxs-lookup"><span data-stu-id="ed3b5-119">string</span></span>   | <span data-ttu-id="ed3b5-120">O número de versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed3b5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed3b5-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="ed3b5-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="ed3b5-122">See also</span></span>

- [<span data-ttu-id="ed3b5-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ed3b5-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ed3b5-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ed3b5-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="ed3b5-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ed3b5-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

