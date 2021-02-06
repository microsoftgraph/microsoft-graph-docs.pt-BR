---
title: Tipo de recurso conditionalAccessLocations
description: Representa locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 153d64d32015fcd6119a4d880bbc786905c39b9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132375"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="eab24-103">Tipo de recurso conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="eab24-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="eab24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eab24-105">Representa locais incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="eab24-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="eab24-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eab24-106">Properties</span></span>

| <span data-ttu-id="eab24-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eab24-107">Property</span></span>     | <span data-ttu-id="eab24-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eab24-108">Type</span></span>        | <span data-ttu-id="eab24-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab24-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eab24-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="eab24-110">includeLocations</span></span> | <span data-ttu-id="eab24-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eab24-111">String collection</span></span> | <span data-ttu-id="eab24-112">IDs de local no escopo da política, a menos que explicitamente `All` excluído, ou `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="eab24-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="eab24-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="eab24-113">excludeLocations</span></span> | <span data-ttu-id="eab24-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eab24-114">String collection</span></span> | <span data-ttu-id="eab24-115">IDs de local excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="eab24-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eab24-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eab24-116">JSON representation</span></span>

<span data-ttu-id="eab24-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eab24-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="eab24-118">Relações</span><span class="sxs-lookup"><span data-stu-id="eab24-118">Relationships</span></span>

<span data-ttu-id="eab24-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eab24-119">None.</span></span>

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

