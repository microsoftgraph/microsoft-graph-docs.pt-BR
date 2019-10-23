---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e163d8f958a400c9c478b0aca865bdfa077c8d60
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638586"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="25cce-103">tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="25cce-103">conditionalAccessApplications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25cce-104">Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="25cce-104">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="25cce-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25cce-105">Properties</span></span>

| <span data-ttu-id="25cce-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25cce-106">Property</span></span> | <span data-ttu-id="25cce-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="25cce-107">Type</span></span> | <span data-ttu-id="25cce-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="25cce-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="25cce-109">includeApplications</span><span class="sxs-lookup"><span data-stu-id="25cce-109">includeApplications</span></span> | <span data-ttu-id="25cce-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cce-110">String collection</span></span> | <span data-ttu-id="25cce-111">A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="25cce-111">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="25cce-112">Também pode ser definido como `All`.</span><span class="sxs-lookup"><span data-stu-id="25cce-112">Can also be set to `All`.</span></span> |
| <span data-ttu-id="25cce-113">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="25cce-113">excludeApplications</span></span> | <span data-ttu-id="25cce-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cce-114">String collection</span></span> | <span data-ttu-id="25cce-115">A lista de IDs de aplicativo explicitamente excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="25cce-115">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="25cce-116">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="25cce-116">includeUserActions</span></span> | <span data-ttu-id="25cce-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25cce-117">String collection</span></span> | <span data-ttu-id="25cce-118">Ações do usuário a serem incluídas ( `urn:user:registersecurityinfo`por exemplo,)</span><span class="sxs-lookup"><span data-stu-id="25cce-118">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="25cce-119">Relações</span><span class="sxs-lookup"><span data-stu-id="25cce-119">Relationships</span></span>

<span data-ttu-id="25cce-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25cce-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25cce-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25cce-121">JSON representation</span></span>

<span data-ttu-id="25cce-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25cce-122">The following is a JSON representation of the resource.</span></span>

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