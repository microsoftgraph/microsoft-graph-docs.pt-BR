---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 95f701151370a6f741e7fa97aa1792ef67ad15d3
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334953"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="083ca-103">tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="083ca-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="083ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="083ca-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="083ca-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="083ca-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="083ca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="083ca-106">Properties</span></span>

| <span data-ttu-id="083ca-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="083ca-107">Property</span></span>            | <span data-ttu-id="083ca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="083ca-108">Type</span></span>     | <span data-ttu-id="083ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="083ca-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="083ca-110">id</span><span class="sxs-lookup"><span data-stu-id="083ca-110">id</span></span>                  | <span data-ttu-id="083ca-111">string</span><span class="sxs-lookup"><span data-stu-id="083ca-111">string</span></span>   | <span data-ttu-id="083ca-112">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="083ca-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="083ca-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="083ca-113">teamsAppId</span></span>          | <span data-ttu-id="083ca-114">string</span><span class="sxs-lookup"><span data-stu-id="083ca-114">string</span></span>   | <span data-ttu-id="083ca-115">A ID do manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="083ca-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="083ca-116">displayName</span><span class="sxs-lookup"><span data-stu-id="083ca-116">displayName</span></span>         | <span data-ttu-id="083ca-117">string</span><span class="sxs-lookup"><span data-stu-id="083ca-117">string</span></span>   | <span data-ttu-id="083ca-118">O nome do aplicativo fornecido pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="083ca-118">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="083ca-119">versão</span><span class="sxs-lookup"><span data-stu-id="083ca-119">version</span></span>             | <span data-ttu-id="083ca-120">string</span><span class="sxs-lookup"><span data-stu-id="083ca-120">string</span></span>   | <span data-ttu-id="083ca-121">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="083ca-121">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="083ca-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="083ca-122">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="083ca-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="083ca-123">See also</span></span>

- [<span data-ttu-id="083ca-124">teamsApp</span><span class="sxs-lookup"><span data-stu-id="083ca-124">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="083ca-125">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="083ca-125">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="083ca-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="083ca-126">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

