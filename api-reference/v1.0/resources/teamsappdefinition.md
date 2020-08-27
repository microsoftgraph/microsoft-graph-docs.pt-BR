---
title: tipo de recurso teamsAppDefinition
description: Representa os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33c16f396d1975b3ffd25de3cf0a8b9f9d7bbf50
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287481"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="ecfbe-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ecfbe-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="ecfbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecfbe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecfbe-105">Representa os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="ecfbe-105">Represents the details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ecfbe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecfbe-106">Properties</span></span>

| <span data-ttu-id="ecfbe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecfbe-107">Property</span></span>            | <span data-ttu-id="ecfbe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecfbe-108">Type</span></span>     | <span data-ttu-id="ecfbe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecfbe-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ecfbe-110">id</span><span class="sxs-lookup"><span data-stu-id="ecfbe-110">id</span></span>                  | <span data-ttu-id="ecfbe-111">string</span><span class="sxs-lookup"><span data-stu-id="ecfbe-111">string</span></span>   | <span data-ttu-id="ecfbe-112">Uma ID exclusiva (não a ID do aplicativo Teams).</span><span class="sxs-lookup"><span data-stu-id="ecfbe-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="ecfbe-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ecfbe-113">teamsAppId</span></span>          | <span data-ttu-id="ecfbe-114">string</span><span class="sxs-lookup"><span data-stu-id="ecfbe-114">string</span></span>   | <span data-ttu-id="ecfbe-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="ecfbe-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="ecfbe-116">publishingState</span></span>| <span data-ttu-id="ecfbe-117">string</span><span class="sxs-lookup"><span data-stu-id="ecfbe-117">string</span></span>|<span data-ttu-id="ecfbe-118">O status publicado de uma versão específica de um aplicativo do teams.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="ecfbe-119">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="ecfbe-119">Possible values are:</span></span></br><span data-ttu-id="ecfbe-120">`submitted` – A versão específica do aplicativo Teams foi enviada e está em revisão.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="ecfbe-121">`published`  — A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="ecfbe-122">`rejected` — A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="ecfbe-123">displayName</span><span class="sxs-lookup"><span data-stu-id="ecfbe-123">displayName</span></span>         | <span data-ttu-id="ecfbe-124">string</span><span class="sxs-lookup"><span data-stu-id="ecfbe-124">string</span></span>   | <span data-ttu-id="ecfbe-125">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="ecfbe-126">versão</span><span class="sxs-lookup"><span data-stu-id="ecfbe-126">version</span></span>             | <span data-ttu-id="ecfbe-127">string</span><span class="sxs-lookup"><span data-stu-id="ecfbe-127">string</span></span>   | <span data-ttu-id="ecfbe-128">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ecfbe-128">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecfbe-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecfbe-129">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="ecfbe-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ecfbe-130">See also</span></span>

- [<span data-ttu-id="ecfbe-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ecfbe-131">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ecfbe-132">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ecfbe-132">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="ecfbe-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ecfbe-133">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
