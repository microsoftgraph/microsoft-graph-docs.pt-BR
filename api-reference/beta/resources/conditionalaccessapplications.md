---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6484ec54b5e39ad2e6b189cc70c05fd666b81297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413513"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="bce27-103">tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="bce27-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="bce27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bce27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bce27-105">Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="bce27-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="bce27-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bce27-106">Properties</span></span>

| <span data-ttu-id="bce27-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bce27-107">Property</span></span> | <span data-ttu-id="bce27-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bce27-108">Type</span></span> | <span data-ttu-id="bce27-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bce27-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="bce27-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="bce27-110">includeApplications</span></span> | <span data-ttu-id="bce27-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bce27-111">String collection</span></span> | <span data-ttu-id="bce27-112">A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="bce27-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="bce27-113">Também pode ser definido como `All`.</span><span class="sxs-lookup"><span data-stu-id="bce27-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="bce27-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="bce27-114">excludeApplications</span></span> | <span data-ttu-id="bce27-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bce27-115">String collection</span></span> | <span data-ttu-id="bce27-116">A lista de IDs de aplicativo explicitamente excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="bce27-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="bce27-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="bce27-117">includeUserActions</span></span> | <span data-ttu-id="bce27-118">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bce27-118">String collection</span></span> | <span data-ttu-id="bce27-119">Ações do usuário a serem incluídas ( `urn:user:registersecurityinfo`por exemplo,)</span><span class="sxs-lookup"><span data-stu-id="bce27-119">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="bce27-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bce27-120">Relationships</span></span>

<span data-ttu-id="bce27-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bce27-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bce27-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bce27-122">JSON representation</span></span>

<span data-ttu-id="bce27-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bce27-123">The following is a JSON representation of the resource.</span></span>

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