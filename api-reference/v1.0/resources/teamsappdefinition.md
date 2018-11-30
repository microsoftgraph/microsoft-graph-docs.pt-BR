---
title: tipo de recurso de teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
ms.openlocfilehash: 34ec74c00dccca48df3b65758e1739cd29b19e7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003814"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="a0745-103">tipo de recurso de teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a0745-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="a0745-104">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="a0745-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a0745-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0745-105">Properties</span></span>

| <span data-ttu-id="a0745-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0745-106">Property</span></span>            | <span data-ttu-id="a0745-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0745-107">Type</span></span>     | <span data-ttu-id="a0745-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0745-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a0745-109">id</span><span class="sxs-lookup"><span data-stu-id="a0745-109">id</span></span>                  | <span data-ttu-id="a0745-110">string</span><span class="sxs-lookup"><span data-stu-id="a0745-110">string</span></span>   | <span data-ttu-id="a0745-111">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="a0745-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="a0745-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a0745-112">teamsAppId</span></span>          | <span data-ttu-id="a0745-113">string</span><span class="sxs-lookup"><span data-stu-id="a0745-113">string</span></span>   | <span data-ttu-id="a0745-114">A identificação de manifesto do aplicativo de equipes.</span><span class="sxs-lookup"><span data-stu-id="a0745-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="a0745-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a0745-115">displayName</span></span>         | <span data-ttu-id="a0745-116">string</span><span class="sxs-lookup"><span data-stu-id="a0745-116">string</span></span>   | <span data-ttu-id="a0745-117">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a0745-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="a0745-118">version</span><span class="sxs-lookup"><span data-stu-id="a0745-118">version</span></span>             | <span data-ttu-id="a0745-119">string</span><span class="sxs-lookup"><span data-stu-id="a0745-119">string</span></span>   | <span data-ttu-id="a0745-120">O número de versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a0745-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0745-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0745-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="a0745-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="a0745-122">See also</span></span>

- [<span data-ttu-id="a0745-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0745-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a0745-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a0745-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="a0745-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0745-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

