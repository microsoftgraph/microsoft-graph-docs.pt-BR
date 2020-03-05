---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 269fe0552c69773fa62b97cf9803b3e0127f655b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507503"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="8a94c-103">tipo de recurso conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="8a94c-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="8a94c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8a94c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a94c-105">Representa usuários, grupos e funções incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="8a94c-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="8a94c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a94c-106">Properties</span></span>

| <span data-ttu-id="8a94c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a94c-107">Property</span></span>     | <span data-ttu-id="8a94c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a94c-108">Type</span></span>        | <span data-ttu-id="8a94c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a94c-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8a94c-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="8a94c-110">includeUsers</span></span> | <span data-ttu-id="8a94c-111">String collection</span><span class="sxs-lookup"><span data-stu-id="8a94c-111">String collection</span></span> | <span data-ttu-id="8a94c-112">IDs de usuário em escopo de política, a menos que `None` explicitamente `All` excluído `GuestsOrExternalUsers`ou ou.</span><span class="sxs-lookup"><span data-stu-id="8a94c-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="8a94c-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="8a94c-113">excludeUsers</span></span> | <span data-ttu-id="8a94c-114">String collection</span><span class="sxs-lookup"><span data-stu-id="8a94c-114">String collection</span></span> | <span data-ttu-id="8a94c-115">IDs de usuário excluídas do escopo da política e `GuestsOrExternalUsers`/ou.</span><span class="sxs-lookup"><span data-stu-id="8a94c-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="8a94c-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="8a94c-116">includeGroups</span></span> | <span data-ttu-id="8a94c-117">String collection</span><span class="sxs-lookup"><span data-stu-id="8a94c-117">String collection</span></span> | <span data-ttu-id="8a94c-118">IDs de grupo em escopo de política, a menos que `All`explicitamente excluído ou.</span><span class="sxs-lookup"><span data-stu-id="8a94c-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="8a94c-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="8a94c-119">excludeGroups</span></span> | <span data-ttu-id="8a94c-120">String collection</span><span class="sxs-lookup"><span data-stu-id="8a94c-120">String collection</span></span> | <span data-ttu-id="8a94c-121">IDs de grupo excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="8a94c-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="8a94c-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="8a94c-122">includeRoles</span></span> | <span data-ttu-id="8a94c-123">String collection</span><span class="sxs-lookup"><span data-stu-id="8a94c-123">String collection</span></span> | <span data-ttu-id="8a94c-124">IDs de função em escopo de política, a menos que `All`explicitamente excluído ou.</span><span class="sxs-lookup"><span data-stu-id="8a94c-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="8a94c-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="8a94c-125">excludeRoles</span></span> | <span data-ttu-id="8a94c-126">String collection</span><span class="sxs-lookup"><span data-stu-id="8a94c-126">String collection</span></span> | <span data-ttu-id="8a94c-127">IDs de função excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="8a94c-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a94c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="8a94c-128">Relationships</span></span>

<span data-ttu-id="8a94c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a94c-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a94c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a94c-130">JSON representation</span></span>

<span data-ttu-id="8a94c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a94c-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeUsers",
    "excludeUsers",
    "includeGroups",
    "excludeGroups",
    "includeRoles",
    "excludeRoles"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessUsers",
  "baseType": null
}-->

```json
{
  "excludeGroups": ["String"],
  "excludeRoles": ["String"],
  "excludeUsers": ["String"],
  "includeGroups": ["String"],
  "includeRoles": ["String"],
  "includeUsers": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessUsers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->