---
title: tipo de recurso conditionalAccessLocations
description: Representa os locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a92d99d7a9e80084b8ec1ce385ce76d1f522b359
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916778"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="92425-103">tipo de recurso conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="92425-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="92425-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92425-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92425-105">Representa os locais incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="92425-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="92425-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92425-106">Properties</span></span>

| <span data-ttu-id="92425-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92425-107">Property</span></span>     | <span data-ttu-id="92425-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="92425-108">Type</span></span>        | <span data-ttu-id="92425-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="92425-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="92425-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="92425-110">includeLocations</span></span> | <span data-ttu-id="92425-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92425-111">String collection</span></span> | <span data-ttu-id="92425-112">IDs de local em escopo de política, a menos `All`que explicitamente `AllTrusted`excluído, ou.</span><span class="sxs-lookup"><span data-stu-id="92425-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="92425-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="92425-113">excludeLocations</span></span> | <span data-ttu-id="92425-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92425-114">String collection</span></span> | <span data-ttu-id="92425-115">IDs de local excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="92425-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92425-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92425-116">JSON representation</span></span>

<span data-ttu-id="92425-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92425-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="92425-118">Relações</span><span class="sxs-lookup"><span data-stu-id="92425-118">Relationships</span></span>

<span data-ttu-id="92425-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92425-119">None.</span></span>

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