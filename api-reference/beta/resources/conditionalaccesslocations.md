---
title: tipo de recurso conditionalAccessLocations
description: Representa os locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6997664eb131664bcaaf571398ed393fb13c987c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638565"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="6679a-103">tipo de recurso conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="6679a-103">conditionalAccessLocations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6679a-104">Representa os locais incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="6679a-104">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="6679a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6679a-105">Properties</span></span>

| <span data-ttu-id="6679a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6679a-106">Property</span></span>     | <span data-ttu-id="6679a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6679a-107">Type</span></span>        | <span data-ttu-id="6679a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6679a-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6679a-109">includeLocations</span><span class="sxs-lookup"><span data-stu-id="6679a-109">includeLocations</span></span> | <span data-ttu-id="6679a-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6679a-110">String collection</span></span> | <span data-ttu-id="6679a-111">IDs de local em escopo de política, a menos `All`que explicitamente `AllTrusted`excluído, ou.</span><span class="sxs-lookup"><span data-stu-id="6679a-111">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="6679a-112">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="6679a-112">excludeLocations</span></span> | <span data-ttu-id="6679a-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6679a-113">String collection</span></span> | <span data-ttu-id="6679a-114">IDs de local excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="6679a-114">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6679a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6679a-115">JSON representation</span></span>

<span data-ttu-id="6679a-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6679a-116">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="6679a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6679a-117">Relationships</span></span>

<span data-ttu-id="6679a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6679a-118">None.</span></span>

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