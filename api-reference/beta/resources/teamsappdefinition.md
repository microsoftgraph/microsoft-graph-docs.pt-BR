---
title: tipo de recurso de teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
ms.openlocfilehash: b2a5b86de67fa1a4ecf673434b13d09c64ebe678
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039685"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="b2c3c-103">tipo de recurso de teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b2c3c-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="b2c3c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b2c3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2c3c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b2c3c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2c3c-106">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2c3c-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b2c3c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2c3c-107">Properties</span></span>

| <span data-ttu-id="b2c3c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2c3c-108">Property</span></span>            | <span data-ttu-id="b2c3c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2c3c-109">Type</span></span>     | <span data-ttu-id="b2c3c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2c3c-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b2c3c-111">id</span><span class="sxs-lookup"><span data-stu-id="b2c3c-111">id</span></span>                  | <span data-ttu-id="b2c3c-112">string</span><span class="sxs-lookup"><span data-stu-id="b2c3c-112">string</span></span>   | <span data-ttu-id="b2c3c-113">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="b2c3c-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="b2c3c-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="b2c3c-114">teamsAppId</span></span>          | <span data-ttu-id="b2c3c-115">string</span><span class="sxs-lookup"><span data-stu-id="b2c3c-115">string</span></span>   | <span data-ttu-id="b2c3c-116">A identificação de manifesto do aplicativo de equipes.</span><span class="sxs-lookup"><span data-stu-id="b2c3c-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="b2c3c-117">displayName</span><span class="sxs-lookup"><span data-stu-id="b2c3c-117">displayName</span></span>         | <span data-ttu-id="b2c3c-118">string</span><span class="sxs-lookup"><span data-stu-id="b2c3c-118">string</span></span>   | <span data-ttu-id="b2c3c-119">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2c3c-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="b2c3c-120">version</span><span class="sxs-lookup"><span data-stu-id="b2c3c-120">version</span></span>             | <span data-ttu-id="b2c3c-121">string</span><span class="sxs-lookup"><span data-stu-id="b2c3c-121">string</span></span>   | <span data-ttu-id="b2c3c-122">O número de versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2c3c-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2c3c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2c3c-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="b2c3c-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="b2c3c-124">See also</span></span>

- [<span data-ttu-id="b2c3c-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b2c3c-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="b2c3c-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b2c3c-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="b2c3c-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b2c3c-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

