---
title: tipo de recurso conditionalAccessLocations
description: Representa os locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09440c789ae98ae2d5eb46de26f56b32bf0ce578
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413405"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="f39f9-103">tipo de recurso conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="f39f9-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="f39f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f39f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f39f9-105">Representa os locais incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="f39f9-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="f39f9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f39f9-106">Properties</span></span>

| <span data-ttu-id="f39f9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f39f9-107">Property</span></span>     | <span data-ttu-id="f39f9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f39f9-108">Type</span></span>        | <span data-ttu-id="f39f9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f39f9-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f39f9-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="f39f9-110">includeLocations</span></span> | <span data-ttu-id="f39f9-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f39f9-111">String collection</span></span> | <span data-ttu-id="f39f9-112">IDs de local em escopo de política, a menos `All`que explicitamente `AllTrusted`excluído, ou.</span><span class="sxs-lookup"><span data-stu-id="f39f9-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="f39f9-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="f39f9-113">excludeLocations</span></span> | <span data-ttu-id="f39f9-114">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f39f9-114">String collection</span></span> | <span data-ttu-id="f39f9-115">IDs de local excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="f39f9-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f39f9-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f39f9-116">JSON representation</span></span>

<span data-ttu-id="f39f9-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f39f9-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="f39f9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f39f9-118">Relationships</span></span>

<span data-ttu-id="f39f9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f39f9-119">None.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->