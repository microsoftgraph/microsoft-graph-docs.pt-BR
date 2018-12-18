---
title: tipo de recurso de teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
ms.openlocfilehash: 43bd4262008a29668739e78d4b598da1e77e3d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351636"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="8d0e1-103">tipo de recurso de teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d0e1-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="8d0e1-104">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d0e1-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8d0e1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d0e1-105">Properties</span></span>

| <span data-ttu-id="8d0e1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d0e1-106">Property</span></span>            | <span data-ttu-id="8d0e1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d0e1-107">Type</span></span>     | <span data-ttu-id="8d0e1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d0e1-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8d0e1-109">id</span><span class="sxs-lookup"><span data-stu-id="8d0e1-109">id</span></span>                  | <span data-ttu-id="8d0e1-110">string</span><span class="sxs-lookup"><span data-stu-id="8d0e1-110">string</span></span>   | <span data-ttu-id="8d0e1-111">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="8d0e1-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="8d0e1-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="8d0e1-112">teamsAppId</span></span>          | <span data-ttu-id="8d0e1-113">string</span><span class="sxs-lookup"><span data-stu-id="8d0e1-113">string</span></span>   | <span data-ttu-id="8d0e1-114">A identificação de manifesto do aplicativo de equipes.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="8d0e1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8d0e1-115">displayName</span></span>         | <span data-ttu-id="8d0e1-116">string</span><span class="sxs-lookup"><span data-stu-id="8d0e1-116">string</span></span>   | <span data-ttu-id="8d0e1-117">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="8d0e1-118">version</span><span class="sxs-lookup"><span data-stu-id="8d0e1-118">version</span></span>             | <span data-ttu-id="8d0e1-119">string</span><span class="sxs-lookup"><span data-stu-id="8d0e1-119">string</span></span>   | <span data-ttu-id="8d0e1-120">O número de versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d0e1-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d0e1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d0e1-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="8d0e1-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="8d0e1-122">See also</span></span>

- [<span data-ttu-id="8d0e1-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d0e1-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="8d0e1-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d0e1-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8d0e1-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8d0e1-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

