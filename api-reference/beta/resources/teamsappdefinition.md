---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6f8cb1f316bf9051dba0fe0ac138d75faf95c8d7
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287488"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="11840-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="11840-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="11840-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11840-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11840-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="11840-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11840-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11840-106">Properties</span></span>

| <span data-ttu-id="11840-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11840-107">Property</span></span>            | <span data-ttu-id="11840-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="11840-108">Type</span></span>     | <span data-ttu-id="11840-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="11840-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="11840-110">id</span><span class="sxs-lookup"><span data-stu-id="11840-110">id</span></span>                  | <span data-ttu-id="11840-111">string</span><span class="sxs-lookup"><span data-stu-id="11840-111">string</span></span>   | <span data-ttu-id="11840-112">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="11840-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="11840-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="11840-113">teamsAppId</span></span>          | <span data-ttu-id="11840-114">string</span><span class="sxs-lookup"><span data-stu-id="11840-114">string</span></span>   | <span data-ttu-id="11840-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="11840-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="11840-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="11840-116">publishingState</span></span>| <span data-ttu-id="11840-117">string</span><span class="sxs-lookup"><span data-stu-id="11840-117">string</span></span>|<span data-ttu-id="11840-118">O status publicado de uma versão específica de um aplicativo do teams.</span><span class="sxs-lookup"><span data-stu-id="11840-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="11840-119">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="11840-119">Possible values are:</span></span></br><span data-ttu-id="11840-120">`submitted` – A versão específica do aplicativo Teams foi enviada e está em revisão.</span><span class="sxs-lookup"><span data-stu-id="11840-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="11840-121">`published`  — A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado.</span><span class="sxs-lookup"><span data-stu-id="11840-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="11840-122">`rejected` — A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="11840-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="11840-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="11840-123">azureADAppId</span></span>        | <span data-ttu-id="11840-124">string</span><span class="sxs-lookup"><span data-stu-id="11840-124">string</span></span>   | <span data-ttu-id="11840-125">O WebApplicationInfo.id do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="11840-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="11840-126">displayName</span><span class="sxs-lookup"><span data-stu-id="11840-126">displayName</span></span>         | <span data-ttu-id="11840-127">string</span><span class="sxs-lookup"><span data-stu-id="11840-127">string</span></span>   | <span data-ttu-id="11840-128">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="11840-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="11840-129">versão</span><span class="sxs-lookup"><span data-stu-id="11840-129">version</span></span>             | <span data-ttu-id="11840-130">string</span><span class="sxs-lookup"><span data-stu-id="11840-130">string</span></span>   | <span data-ttu-id="11840-131">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11840-131">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11840-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11840-132">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="11840-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="11840-133">See also</span></span>

- [<span data-ttu-id="11840-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="11840-134">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="11840-135">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="11840-135">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="11840-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="11840-136">teamsTab</span></span>](../resources/teamstab.md)

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
