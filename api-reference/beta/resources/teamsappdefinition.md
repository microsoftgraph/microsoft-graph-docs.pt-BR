---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d4d9cb74777985dd28988e1ebc417ee564932865
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046591"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="a10e4-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a10e4-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="a10e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a10e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a10e4-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="a10e4-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a10e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a10e4-106">Properties</span></span>

| <span data-ttu-id="a10e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a10e4-107">Property</span></span>            | <span data-ttu-id="a10e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a10e4-108">Type</span></span>     | <span data-ttu-id="a10e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a10e4-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a10e4-110">id</span><span class="sxs-lookup"><span data-stu-id="a10e4-110">id</span></span>                  | <span data-ttu-id="a10e4-111">string</span><span class="sxs-lookup"><span data-stu-id="a10e4-111">string</span></span>   | <span data-ttu-id="a10e4-112">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="a10e4-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="a10e4-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a10e4-113">teamsAppId</span></span>          | <span data-ttu-id="a10e4-114">string</span><span class="sxs-lookup"><span data-stu-id="a10e4-114">string</span></span>   | <span data-ttu-id="a10e4-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="a10e4-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="a10e4-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="a10e4-116">publishingState</span></span>| <span data-ttu-id="a10e4-117">string</span><span class="sxs-lookup"><span data-stu-id="a10e4-117">string</span></span>|<span data-ttu-id="a10e4-118">O status publicado de uma versão específica de um aplicativo do teams.</span><span class="sxs-lookup"><span data-stu-id="a10e4-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="a10e4-119">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="a10e4-119">Possible values are:</span></span></br><span data-ttu-id="a10e4-120">`submitted` – A versão específica do aplicativo Teams foi enviada e está em revisão.</span><span class="sxs-lookup"><span data-stu-id="a10e4-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="a10e4-121">`published`  — A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado.</span><span class="sxs-lookup"><span data-stu-id="a10e4-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="a10e4-122">`rejected` — A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a10e4-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="a10e4-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="a10e4-123">azureADAppId</span></span>        | <span data-ttu-id="a10e4-124">string</span><span class="sxs-lookup"><span data-stu-id="a10e4-124">string</span></span>   | <span data-ttu-id="a10e4-125">O WebApplicationInfo.id do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="a10e4-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="a10e4-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a10e4-126">displayName</span></span>         | <span data-ttu-id="a10e4-127">string</span><span class="sxs-lookup"><span data-stu-id="a10e4-127">string</span></span>   | <span data-ttu-id="a10e4-128">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a10e4-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="a10e4-129">versão</span><span class="sxs-lookup"><span data-stu-id="a10e4-129">version</span></span>             | <span data-ttu-id="a10e4-130">string</span><span class="sxs-lookup"><span data-stu-id="a10e4-130">string</span></span>   | <span data-ttu-id="a10e4-131">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a10e4-131">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a10e4-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a10e4-132">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a10e4-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="a10e4-133">See also</span></span>

- [<span data-ttu-id="a10e4-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a10e4-134">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a10e4-135">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a10e4-135">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="a10e4-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a10e4-136">teamsTab</span></span>](../resources/teamstab.md)

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


