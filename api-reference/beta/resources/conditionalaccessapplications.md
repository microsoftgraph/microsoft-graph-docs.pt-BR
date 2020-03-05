---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4e66618a8dbf6d5d29ca3b5c08a9b7bd10e05ded
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507566"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="c0043-103">tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="c0043-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="c0043-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c0043-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0043-105">Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="c0043-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="c0043-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0043-106">Properties</span></span>

| <span data-ttu-id="c0043-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0043-107">Property</span></span> | <span data-ttu-id="c0043-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0043-108">Type</span></span> | <span data-ttu-id="c0043-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0043-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="c0043-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="c0043-110">includeApplications</span></span> | <span data-ttu-id="c0043-111">String collection</span><span class="sxs-lookup"><span data-stu-id="c0043-111">String collection</span></span> | <span data-ttu-id="c0043-112">A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="c0043-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="c0043-113">Também pode ser definido como `All`.</span><span class="sxs-lookup"><span data-stu-id="c0043-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="c0043-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="c0043-114">excludeApplications</span></span> | <span data-ttu-id="c0043-115">String collection</span><span class="sxs-lookup"><span data-stu-id="c0043-115">String collection</span></span> | <span data-ttu-id="c0043-116">A lista de IDs de aplicativo explicitamente excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="c0043-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="c0043-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="c0043-117">includeUserActions</span></span> | <span data-ttu-id="c0043-118">String collection</span><span class="sxs-lookup"><span data-stu-id="c0043-118">String collection</span></span> | <span data-ttu-id="c0043-119">Ações do usuário a serem incluídas ( `urn:user:registersecurityinfo`por exemplo,)</span><span class="sxs-lookup"><span data-stu-id="c0043-119">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="c0043-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c0043-120">Relationships</span></span>

<span data-ttu-id="c0043-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0043-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0043-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0043-122">JSON representation</span></span>

<span data-ttu-id="c0043-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0043-123">The following is a JSON representation of the resource.</span></span>

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