---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5fd771d1fb38de5354c74778f5eae798ccc91e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706112"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="dd939-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="dd939-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="dd939-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd939-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd939-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd939-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dd939-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd939-106">Properties</span></span>

| <span data-ttu-id="dd939-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd939-107">Property</span></span>            | <span data-ttu-id="dd939-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd939-108">Type</span></span>     | <span data-ttu-id="dd939-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd939-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="dd939-110">id</span><span class="sxs-lookup"><span data-stu-id="dd939-110">id</span></span>                  | <span data-ttu-id="dd939-111">string</span><span class="sxs-lookup"><span data-stu-id="dd939-111">string</span></span>   | <span data-ttu-id="dd939-112">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="dd939-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="dd939-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="dd939-113">teamsAppId</span></span>          | <span data-ttu-id="dd939-114">string</span><span class="sxs-lookup"><span data-stu-id="dd939-114">string</span></span>   | <span data-ttu-id="dd939-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="dd939-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="dd939-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="dd939-116">publishingState</span></span>| <span data-ttu-id="dd939-117">string</span><span class="sxs-lookup"><span data-stu-id="dd939-117">string</span></span>|<span data-ttu-id="dd939-118">O status publicado de uma versão específica de um aplicativo do teams.</span><span class="sxs-lookup"><span data-stu-id="dd939-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="dd939-119">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="dd939-119">Possible values are:</span></span></br><span data-ttu-id="dd939-120">`submitted` – A versão específica do aplicativo Teams foi enviada e está em revisão.</span><span class="sxs-lookup"><span data-stu-id="dd939-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="dd939-121">`published`  — A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado.</span><span class="sxs-lookup"><span data-stu-id="dd939-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="dd939-122">`rejected` — A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="dd939-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="dd939-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="dd939-123">azureADAppId</span></span>        | <span data-ttu-id="dd939-124">string</span><span class="sxs-lookup"><span data-stu-id="dd939-124">string</span></span>   | <span data-ttu-id="dd939-125">O WebApplicationInfo.id do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="dd939-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="dd939-126">displayName</span><span class="sxs-lookup"><span data-stu-id="dd939-126">displayName</span></span>         | <span data-ttu-id="dd939-127">string</span><span class="sxs-lookup"><span data-stu-id="dd939-127">string</span></span>   | <span data-ttu-id="dd939-128">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="dd939-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="dd939-129">versão</span><span class="sxs-lookup"><span data-stu-id="dd939-129">version</span></span>             | <span data-ttu-id="dd939-130">string</span><span class="sxs-lookup"><span data-stu-id="dd939-130">string</span></span>   | <span data-ttu-id="dd939-131">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dd939-131">The version number of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd939-132">Relações</span><span class="sxs-lookup"><span data-stu-id="dd939-132">Relationships</span></span>

| <span data-ttu-id="dd939-133">Relação</span><span class="sxs-lookup"><span data-stu-id="dd939-133">Relationship</span></span> | <span data-ttu-id="dd939-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd939-134">Type</span></span>   | <span data-ttu-id="dd939-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd939-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dd939-136">bot</span><span class="sxs-lookup"><span data-stu-id="dd939-136">bot</span></span>|[<span data-ttu-id="dd939-137">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="dd939-137">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="dd939-138">Os detalhes do bot especificado no manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="dd939-138">The details of the bot specified in the Teams App manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd939-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd939-139">JSON representation</span></span>

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
  "version": "1.0.0"
}
```

## <a name="see-also"></a><span data-ttu-id="dd939-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="dd939-140">See also</span></span>

- [<span data-ttu-id="dd939-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dd939-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="dd939-142">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="dd939-142">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="dd939-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dd939-143">teamsTab</span></span>](../resources/teamstab.md)

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


