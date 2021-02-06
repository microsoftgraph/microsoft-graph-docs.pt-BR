---
title: Tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6214c3daacf580aaffa01a93be2b2c785c03f4fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128579"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="cd529-103">Tipo de recurso conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="cd529-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="cd529-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd529-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd529-105">Representa usuários, grupos e funções incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="cd529-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="cd529-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd529-106">Properties</span></span>

| <span data-ttu-id="cd529-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd529-107">Property</span></span>     | <span data-ttu-id="cd529-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd529-108">Type</span></span>        | <span data-ttu-id="cd529-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd529-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cd529-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="cd529-110">includeUsers</span></span> | <span data-ttu-id="cd529-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd529-111">String collection</span></span> | <span data-ttu-id="cd529-112">IDs de usuário no escopo da política, a menos que explicitamente excluídos, `None` ou `All` ou `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="cd529-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="cd529-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="cd529-113">excludeUsers</span></span> | <span data-ttu-id="cd529-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd529-114">String collection</span></span> | <span data-ttu-id="cd529-115">IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="cd529-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="cd529-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="cd529-116">includeGroups</span></span> | <span data-ttu-id="cd529-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd529-117">String collection</span></span> | <span data-ttu-id="cd529-118">IDs de grupo no escopo da política, a menos que explicitamente excluídas, ou `All` .</span><span class="sxs-lookup"><span data-stu-id="cd529-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="cd529-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="cd529-119">excludeGroups</span></span> | <span data-ttu-id="cd529-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd529-120">String collection</span></span> | <span data-ttu-id="cd529-121">IDs de grupo excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="cd529-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="cd529-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="cd529-122">includeRoles</span></span> | <span data-ttu-id="cd529-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd529-123">String collection</span></span> | <span data-ttu-id="cd529-124">IDs de função no escopo da política, a menos que explicitamente excluído, ou `All` .</span><span class="sxs-lookup"><span data-stu-id="cd529-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="cd529-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="cd529-125">excludeRoles</span></span> | <span data-ttu-id="cd529-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd529-126">String collection</span></span> | <span data-ttu-id="cd529-127">IDs de função excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="cd529-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cd529-128">Relações</span><span class="sxs-lookup"><span data-stu-id="cd529-128">Relationships</span></span>

<span data-ttu-id="cd529-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd529-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd529-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd529-130">JSON representation</span></span>

<span data-ttu-id="cd529-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd529-131">The following is a JSON representation of the resource.</span></span>

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

