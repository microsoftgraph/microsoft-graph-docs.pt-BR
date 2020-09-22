---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d5a25b287d4f82aaaf9a7773893f96a02a7cf124
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085182"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="b3e9a-103">tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="b3e9a-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="b3e9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3e9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e9a-105">Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="b3e9a-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b3e9a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3e9a-106">Properties</span></span>

| <span data-ttu-id="b3e9a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3e9a-107">Property</span></span> | <span data-ttu-id="b3e9a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3e9a-108">Type</span></span> | <span data-ttu-id="b3e9a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3e9a-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="b3e9a-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="b3e9a-110">includeApplications</span></span> | <span data-ttu-id="b3e9a-111">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b3e9a-111">String collection</span></span> | <span data-ttu-id="b3e9a-112">A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="b3e9a-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="b3e9a-113">Também pode ser definido como `All` .</span><span class="sxs-lookup"><span data-stu-id="b3e9a-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="b3e9a-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="b3e9a-114">excludeApplications</span></span> | <span data-ttu-id="b3e9a-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b3e9a-115">String collection</span></span> | <span data-ttu-id="b3e9a-116">A lista de IDs de aplicativo explicitamente excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="b3e9a-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="b3e9a-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="b3e9a-117">includeUserActions</span></span> | <span data-ttu-id="b3e9a-118">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b3e9a-118">String collection</span></span> | <span data-ttu-id="b3e9a-119">Ações do usuário a serem incluídas (por exemplo, `urn:user:registersecurityinfo` )</span><span class="sxs-lookup"><span data-stu-id="b3e9a-119">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="b3e9a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b3e9a-120">Relationships</span></span>

<span data-ttu-id="b3e9a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3e9a-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3e9a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3e9a-122">JSON representation</span></span>

<span data-ttu-id="b3e9a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3e9a-123">The following is a JSON representation of the resource.</span></span>

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

