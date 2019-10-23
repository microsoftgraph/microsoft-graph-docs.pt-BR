---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e54c5b018331952776b36a0ab3c07be88c2be7c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638474"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="93899-103">tipo de recurso conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="93899-103">conditionalAccessUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93899-104">Representa usuários, grupos e funções incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="93899-104">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="93899-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93899-105">Properties</span></span>

| <span data-ttu-id="93899-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93899-106">Property</span></span>     | <span data-ttu-id="93899-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="93899-107">Type</span></span>        | <span data-ttu-id="93899-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="93899-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="93899-109">includeUsers</span><span class="sxs-lookup"><span data-stu-id="93899-109">includeUsers</span></span> | <span data-ttu-id="93899-110">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93899-110">String collection</span></span> | <span data-ttu-id="93899-111">IDs de usuário em escopo de política, a menos que `None` explicitamente `All` excluído `GuestsOrExternalUsers`ou ou.</span><span class="sxs-lookup"><span data-stu-id="93899-111">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="93899-112">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="93899-112">excludeUsers</span></span> | <span data-ttu-id="93899-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93899-113">String collection</span></span> | <span data-ttu-id="93899-114">IDs de usuário excluídas do escopo da política e `GuestsOrExternalUsers`/ou.</span><span class="sxs-lookup"><span data-stu-id="93899-114">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="93899-115">includeGroups</span><span class="sxs-lookup"><span data-stu-id="93899-115">includeGroups</span></span> | <span data-ttu-id="93899-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93899-116">String collection</span></span> | <span data-ttu-id="93899-117">IDs de grupo em escopo de política, a menos que `All`explicitamente excluído ou.</span><span class="sxs-lookup"><span data-stu-id="93899-117">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="93899-118">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="93899-118">excludeGroups</span></span> | <span data-ttu-id="93899-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93899-119">String collection</span></span> | <span data-ttu-id="93899-120">IDs de grupo excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="93899-120">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="93899-121">includeRoles</span><span class="sxs-lookup"><span data-stu-id="93899-121">includeRoles</span></span> | <span data-ttu-id="93899-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93899-122">String collection</span></span> | <span data-ttu-id="93899-123">IDs de função em escopo de política, a menos que `All`explicitamente excluído ou.</span><span class="sxs-lookup"><span data-stu-id="93899-123">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="93899-124">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="93899-124">excludeRoles</span></span> | <span data-ttu-id="93899-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93899-125">String collection</span></span> | <span data-ttu-id="93899-126">IDs de função excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="93899-126">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="93899-127">Relações</span><span class="sxs-lookup"><span data-stu-id="93899-127">Relationships</span></span>

<span data-ttu-id="93899-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93899-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93899-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93899-129">JSON representation</span></span>

<span data-ttu-id="93899-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93899-130">The following is a JSON representation of the resource.</span></span>

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