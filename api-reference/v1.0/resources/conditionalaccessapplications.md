---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a9794a274b876ba93cc3fdbe14ea7731776daa3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057042"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="bf76d-103">tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="bf76d-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="bf76d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf76d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf76d-105">Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="bf76d-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="bf76d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf76d-106">Properties</span></span>

| <span data-ttu-id="bf76d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf76d-107">Property</span></span>     | <span data-ttu-id="bf76d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf76d-108">Type</span></span>        | <span data-ttu-id="bf76d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf76d-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bf76d-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="bf76d-110">includeApplications</span></span> | <span data-ttu-id="bf76d-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf76d-111">String collection</span></span> | <span data-ttu-id="bf76d-112">A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="bf76d-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="bf76d-113">Também pode ser definido como `All` .</span><span class="sxs-lookup"><span data-stu-id="bf76d-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="bf76d-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="bf76d-114">excludeApplications</span></span> | <span data-ttu-id="bf76d-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf76d-115">String collection</span></span> | <span data-ttu-id="bf76d-116">A lista de IDs de aplicativo explicitamente excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="bf76d-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="bf76d-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="bf76d-117">includeUserActions</span></span> | <span data-ttu-id="bf76d-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf76d-118">String collection</span></span> | <span data-ttu-id="bf76d-119">Ações do usuário a serem incluídas.</span><span class="sxs-lookup"><span data-stu-id="bf76d-119">User actions to include.</span></span> <span data-ttu-id="bf76d-120">Por exemplo, `urn:user:registersecurityinfo`</span><span class="sxs-lookup"><span data-stu-id="bf76d-120">For example, `urn:user:registersecurityinfo`</span></span> |

## <a name="relationships"></a><span data-ttu-id="bf76d-121">Relações</span><span class="sxs-lookup"><span data-stu-id="bf76d-121">Relationships</span></span>

<span data-ttu-id="bf76d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf76d-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf76d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf76d-123">JSON representation</span></span>

<span data-ttu-id="bf76d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf76d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

