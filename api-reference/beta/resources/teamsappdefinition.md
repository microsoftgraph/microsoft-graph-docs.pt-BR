---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b8dd3e7b3e50ed5642aeb23076705f4995e27759
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272707"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="b71a3-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b71a3-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="b71a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b71a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b71a3-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="b71a3-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b71a3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b71a3-106">Properties</span></span>

| <span data-ttu-id="b71a3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b71a3-107">Property</span></span>            | <span data-ttu-id="b71a3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b71a3-108">Type</span></span>     | <span data-ttu-id="b71a3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b71a3-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b71a3-110">id</span><span class="sxs-lookup"><span data-stu-id="b71a3-110">id</span></span>                  | <span data-ttu-id="b71a3-111">string</span><span class="sxs-lookup"><span data-stu-id="b71a3-111">string</span></span>   | <span data-ttu-id="b71a3-112">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="b71a3-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="b71a3-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="b71a3-113">teamsAppId</span></span>          | <span data-ttu-id="b71a3-114">string</span><span class="sxs-lookup"><span data-stu-id="b71a3-114">string</span></span>   | <span data-ttu-id="b71a3-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="b71a3-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="b71a3-116">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="b71a3-116">azureADAppId</span></span>        | <span data-ttu-id="b71a3-117">string</span><span class="sxs-lookup"><span data-stu-id="b71a3-117">string</span></span>   | <span data-ttu-id="b71a3-118">O WebApplicationInfo.id do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="b71a3-118">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="b71a3-119">displayName</span><span class="sxs-lookup"><span data-stu-id="b71a3-119">displayName</span></span>         | <span data-ttu-id="b71a3-120">string</span><span class="sxs-lookup"><span data-stu-id="b71a3-120">string</span></span>   | <span data-ttu-id="b71a3-121">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b71a3-121">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="b71a3-122">versão</span><span class="sxs-lookup"><span data-stu-id="b71a3-122">version</span></span>             | <span data-ttu-id="b71a3-123">string</span><span class="sxs-lookup"><span data-stu-id="b71a3-123">string</span></span>   | <span data-ttu-id="b71a3-124">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b71a3-124">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b71a3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b71a3-125">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b71a3-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="b71a3-126">See also</span></span>

- [<span data-ttu-id="b71a3-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b71a3-127">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="b71a3-128">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b71a3-128">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="b71a3-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b71a3-129">teamsTab</span></span>](../resources/teamstab.md)

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

