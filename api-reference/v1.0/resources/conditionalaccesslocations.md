---
title: Tipo de recurso conditionalAccessLocations
description: Representa locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 670f07e22b2027c74a79eaca505c624c04c19621
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132111"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="08032-103">Tipo de recurso conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="08032-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="08032-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08032-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08032-105">Representa locais incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="08032-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="08032-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08032-106">Properties</span></span>

| <span data-ttu-id="08032-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08032-107">Property</span></span>     | <span data-ttu-id="08032-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="08032-108">Type</span></span>        | <span data-ttu-id="08032-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08032-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="08032-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="08032-110">includeLocations</span></span> | <span data-ttu-id="08032-111">String collection</span><span class="sxs-lookup"><span data-stu-id="08032-111">String collection</span></span> | <span data-ttu-id="08032-112">IDs de local no escopo da política, a menos que explicitamente `All` excluído, ou `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="08032-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="08032-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="08032-113">excludeLocations</span></span> | <span data-ttu-id="08032-114">String collection</span><span class="sxs-lookup"><span data-stu-id="08032-114">String collection</span></span> | <span data-ttu-id="08032-115">IDs de local excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="08032-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08032-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08032-116">JSON representation</span></span>

<span data-ttu-id="08032-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08032-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="08032-118">Relações</span><span class="sxs-lookup"><span data-stu-id="08032-118">Relationships</span></span>

<span data-ttu-id="08032-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08032-119">None.</span></span>

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

