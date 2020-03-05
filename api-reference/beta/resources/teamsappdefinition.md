---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a3c40433a1be214141dff8eda99142a96be0a003
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519915"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="01252-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="01252-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="01252-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="01252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01252-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="01252-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="01252-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01252-106">Properties</span></span>

| <span data-ttu-id="01252-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01252-107">Property</span></span>            | <span data-ttu-id="01252-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="01252-108">Type</span></span>     | <span data-ttu-id="01252-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="01252-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="01252-110">id</span><span class="sxs-lookup"><span data-stu-id="01252-110">id</span></span>                  | <span data-ttu-id="01252-111">string</span><span class="sxs-lookup"><span data-stu-id="01252-111">string</span></span>   | <span data-ttu-id="01252-112">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="01252-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="01252-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="01252-113">teamsAppId</span></span>          | <span data-ttu-id="01252-114">string</span><span class="sxs-lookup"><span data-stu-id="01252-114">string</span></span>   | <span data-ttu-id="01252-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="01252-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="01252-116">displayName</span><span class="sxs-lookup"><span data-stu-id="01252-116">displayName</span></span>         | <span data-ttu-id="01252-117">string</span><span class="sxs-lookup"><span data-stu-id="01252-117">string</span></span>   | <span data-ttu-id="01252-118">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="01252-118">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="01252-119">versão</span><span class="sxs-lookup"><span data-stu-id="01252-119">version</span></span>             | <span data-ttu-id="01252-120">string</span><span class="sxs-lookup"><span data-stu-id="01252-120">string</span></span>   | <span data-ttu-id="01252-121">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="01252-121">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="01252-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01252-122">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="01252-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="01252-123">See also</span></span>

- [<span data-ttu-id="01252-124">teamsApp</span><span class="sxs-lookup"><span data-stu-id="01252-124">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="01252-125">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="01252-125">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="01252-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01252-126">teamsTab</span></span>](../resources/teamstab.md)

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

