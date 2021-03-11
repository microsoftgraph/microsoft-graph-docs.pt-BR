---
title: Tipo de recurso teamsAppDefinition
description: Representa os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a43083e1f7fb717e2d54caef4017aeae97d9392
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625930"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="9af07-103">Tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="9af07-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="9af07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9af07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9af07-105">Representa os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="9af07-105">Represents the details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9af07-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9af07-106">Properties</span></span>

| <span data-ttu-id="9af07-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9af07-107">Property</span></span>            | <span data-ttu-id="9af07-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9af07-108">Type</span></span>     | <span data-ttu-id="9af07-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9af07-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="9af07-110">id</span><span class="sxs-lookup"><span data-stu-id="9af07-110">id</span></span>                  | <span data-ttu-id="9af07-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af07-111">string</span></span>   | <span data-ttu-id="9af07-112">Uma ID exclusiva (não a ID do aplicativo do Teams).</span><span class="sxs-lookup"><span data-stu-id="9af07-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="9af07-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="9af07-113">teamsAppId</span></span>          | <span data-ttu-id="9af07-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af07-114">string</span></span>   | <span data-ttu-id="9af07-115">A ID do manifesto do aplicativo teams.</span><span class="sxs-lookup"><span data-stu-id="9af07-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="9af07-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="9af07-116">publishingState</span></span>| <span data-ttu-id="9af07-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af07-117">string</span></span>|<span data-ttu-id="9af07-118">O status publicado de uma versão específica de um aplicativo do Teams.</span><span class="sxs-lookup"><span data-stu-id="9af07-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="9af07-119">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="9af07-119">Possible values are:</span></span></br><span data-ttu-id="9af07-120">`submitted` — A versão específica do aplicativo teams foi enviada e está sob revisão.</span><span class="sxs-lookup"><span data-stu-id="9af07-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="9af07-121">`published`  — A solicitação para publicar a versão específica do aplicativo teams foi aprovada pelo administrador e o aplicativo é publicado.</span><span class="sxs-lookup"><span data-stu-id="9af07-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="9af07-122">`rejected` — A solicitação para publicar a versão específica do aplicativo teams foi rejeitada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9af07-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="9af07-123">displayName</span><span class="sxs-lookup"><span data-stu-id="9af07-123">displayName</span></span>         | <span data-ttu-id="9af07-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af07-124">string</span></span>   | <span data-ttu-id="9af07-125">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9af07-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="9af07-126">versão</span><span class="sxs-lookup"><span data-stu-id="9af07-126">version</span></span>             | <span data-ttu-id="9af07-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af07-127">string</span></span>   | <span data-ttu-id="9af07-128">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9af07-128">The version number of the application.</span></span> |
| <span data-ttu-id="9af07-129">shortDescription</span><span class="sxs-lookup"><span data-stu-id="9af07-129">shortDescription</span></span>    | <span data-ttu-id="9af07-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af07-130">string</span></span>   | <span data-ttu-id="9af07-131">Descrição curta do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9af07-131">Short description of the application.</span></span> |
| <span data-ttu-id="9af07-132">description</span><span class="sxs-lookup"><span data-stu-id="9af07-132">description</span></span>         | <span data-ttu-id="9af07-133">string</span><span class="sxs-lookup"><span data-stu-id="9af07-133">string</span></span>   | <span data-ttu-id="9af07-134">Descrição detalhada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9af07-134">Verbose description of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9af07-135">Relações</span><span class="sxs-lookup"><span data-stu-id="9af07-135">Relationships</span></span>

| <span data-ttu-id="9af07-136">Relação</span><span class="sxs-lookup"><span data-stu-id="9af07-136">Relationship</span></span> | <span data-ttu-id="9af07-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="9af07-137">Type</span></span>   | <span data-ttu-id="9af07-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="9af07-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9af07-139">bot</span><span class="sxs-lookup"><span data-stu-id="9af07-139">bot</span></span>|[<span data-ttu-id="9af07-140">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="9af07-140">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="9af07-141">Os detalhes do bot especificados no manifesto do aplicativo teams.</span><span class="sxs-lookup"><span data-stu-id="9af07-141">The details of the bot specified in the Teams app manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9af07-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9af07-142">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9af07-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="9af07-143">See also</span></span>

- [<span data-ttu-id="9af07-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9af07-144">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="9af07-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9af07-145">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="9af07-146">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9af07-146">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

