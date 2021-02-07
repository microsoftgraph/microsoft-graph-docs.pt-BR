---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações do usuário incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 42ceafb6c786666378d1327ecd158a04559d7f0d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132157"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="d3bdb-103">Tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="d3bdb-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="d3bdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3bdb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3bdb-105">Representa os aplicativos e as ações do usuário incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="d3bdb-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d3bdb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3bdb-106">Properties</span></span>

| <span data-ttu-id="d3bdb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3bdb-107">Property</span></span>     | <span data-ttu-id="d3bdb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3bdb-108">Type</span></span>        | <span data-ttu-id="d3bdb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3bdb-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d3bdb-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="d3bdb-110">includeApplications</span></span> | <span data-ttu-id="d3bdb-111">String collection</span><span class="sxs-lookup"><span data-stu-id="d3bdb-111">String collection</span></span> | <span data-ttu-id="d3bdb-112">A lista de IDs de aplicativos a que a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="d3bdb-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="d3bdb-113">Também pode ser definido como `All` .</span><span class="sxs-lookup"><span data-stu-id="d3bdb-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="d3bdb-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="d3bdb-114">excludeApplications</span></span> | <span data-ttu-id="d3bdb-115">String collection</span><span class="sxs-lookup"><span data-stu-id="d3bdb-115">String collection</span></span> | <span data-ttu-id="d3bdb-116">A lista de IDs de aplicativo explicitamente excluída da política.</span><span class="sxs-lookup"><span data-stu-id="d3bdb-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="d3bdb-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="d3bdb-117">includeUserActions</span></span> | <span data-ttu-id="d3bdb-118">String collection</span><span class="sxs-lookup"><span data-stu-id="d3bdb-118">String collection</span></span> | <span data-ttu-id="d3bdb-119">Ações do usuário a incluir.</span><span class="sxs-lookup"><span data-stu-id="d3bdb-119">User actions to include.</span></span> <span data-ttu-id="d3bdb-120">Por exemplo, `urn:user:registersecurityinfo`</span><span class="sxs-lookup"><span data-stu-id="d3bdb-120">For example, `urn:user:registersecurityinfo`</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3bdb-121">Relações</span><span class="sxs-lookup"><span data-stu-id="d3bdb-121">Relationships</span></span>

<span data-ttu-id="d3bdb-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3bdb-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3bdb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3bdb-123">JSON representation</span></span>

<span data-ttu-id="d3bdb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3bdb-124">The following is a JSON representation of the resource.</span></span>

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

