---
title: tipo de recurso conditionalAccessLocations
description: Representa os locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5378764f36bf5fed858755a475fd85a400a2fed
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384407"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="5549b-103">tipo de recurso conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="5549b-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="5549b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5549b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5549b-105">Representa os locais incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5549b-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5549b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5549b-106">Properties</span></span>

| <span data-ttu-id="5549b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5549b-107">Property</span></span>     | <span data-ttu-id="5549b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5549b-108">Type</span></span>        | <span data-ttu-id="5549b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5549b-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5549b-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="5549b-110">includeLocations</span></span> | <span data-ttu-id="5549b-111">String collection</span><span class="sxs-lookup"><span data-stu-id="5549b-111">String collection</span></span> | <span data-ttu-id="5549b-112">IDs de local em escopo de política, a menos que explicitamente excluído, `All` ou `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="5549b-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="5549b-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="5549b-113">excludeLocations</span></span> | <span data-ttu-id="5549b-114">String collection</span><span class="sxs-lookup"><span data-stu-id="5549b-114">String collection</span></span> | <span data-ttu-id="5549b-115">IDs de local excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="5549b-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5549b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5549b-116">JSON representation</span></span>

<span data-ttu-id="5549b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5549b-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="5549b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5549b-118">Relationships</span></span>

<span data-ttu-id="5549b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5549b-119">None.</span></span>

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
