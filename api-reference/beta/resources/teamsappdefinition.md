---
title: tipo de recurso de teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a13f6ffd4ca5385b9e264f8b8a5b8bddfe0a1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851293"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="577d8-103">tipo de recurso de teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="577d8-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="577d8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="577d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="577d8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="577d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="577d8-106">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="577d8-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="577d8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="577d8-107">Properties</span></span>

| <span data-ttu-id="577d8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="577d8-108">Property</span></span>            | <span data-ttu-id="577d8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="577d8-109">Type</span></span>     | <span data-ttu-id="577d8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="577d8-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="577d8-111">id</span><span class="sxs-lookup"><span data-stu-id="577d8-111">id</span></span>                  | <span data-ttu-id="577d8-112">string</span><span class="sxs-lookup"><span data-stu-id="577d8-112">string</span></span>   | <span data-ttu-id="577d8-113">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="577d8-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="577d8-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="577d8-114">teamsAppId</span></span>          | <span data-ttu-id="577d8-115">string</span><span class="sxs-lookup"><span data-stu-id="577d8-115">string</span></span>   | <span data-ttu-id="577d8-116">A identificação de manifesto do aplicativo de equipes.</span><span class="sxs-lookup"><span data-stu-id="577d8-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="577d8-117">displayName</span><span class="sxs-lookup"><span data-stu-id="577d8-117">displayName</span></span>         | <span data-ttu-id="577d8-118">string</span><span class="sxs-lookup"><span data-stu-id="577d8-118">string</span></span>   | <span data-ttu-id="577d8-119">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="577d8-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="577d8-120">version</span><span class="sxs-lookup"><span data-stu-id="577d8-120">version</span></span>             | <span data-ttu-id="577d8-121">string</span><span class="sxs-lookup"><span data-stu-id="577d8-121">string</span></span>   | <span data-ttu-id="577d8-122">O número de versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="577d8-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="577d8-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="577d8-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="577d8-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="577d8-124">See also</span></span>

- [<span data-ttu-id="577d8-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="577d8-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="577d8-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="577d8-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="577d8-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="577d8-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

