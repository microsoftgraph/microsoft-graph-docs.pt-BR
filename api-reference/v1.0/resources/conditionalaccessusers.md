---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 460b14d88fcf153935948784c08a6d0a03d33553
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384433"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="feb19-103">tipo de recurso conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="feb19-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="feb19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="feb19-105">Representa usuários, grupos e funções incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="feb19-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="feb19-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feb19-106">Properties</span></span>

| <span data-ttu-id="feb19-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feb19-107">Property</span></span>     | <span data-ttu-id="feb19-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="feb19-108">Type</span></span>        | <span data-ttu-id="feb19-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="feb19-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="feb19-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="feb19-110">includeUsers</span></span> | <span data-ttu-id="feb19-111">String collection</span><span class="sxs-lookup"><span data-stu-id="feb19-111">String collection</span></span> | <span data-ttu-id="feb19-112">IDs de usuário em escopo de política, a menos que explicitamente excluído ou ou `None` `All` `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="feb19-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="feb19-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="feb19-113">excludeUsers</span></span> | <span data-ttu-id="feb19-114">String collection</span><span class="sxs-lookup"><span data-stu-id="feb19-114">String collection</span></span> | <span data-ttu-id="feb19-115">IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="feb19-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="feb19-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="feb19-116">includeGroups</span></span> | <span data-ttu-id="feb19-117">String collection</span><span class="sxs-lookup"><span data-stu-id="feb19-117">String collection</span></span> | <span data-ttu-id="feb19-118">IDs de grupo em escopo de política, a menos que explicitamente excluído ou `All` .</span><span class="sxs-lookup"><span data-stu-id="feb19-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="feb19-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="feb19-119">excludeGroups</span></span> | <span data-ttu-id="feb19-120">String collection</span><span class="sxs-lookup"><span data-stu-id="feb19-120">String collection</span></span> | <span data-ttu-id="feb19-121">IDs de grupo excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="feb19-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="feb19-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="feb19-122">includeRoles</span></span> | <span data-ttu-id="feb19-123">String collection</span><span class="sxs-lookup"><span data-stu-id="feb19-123">String collection</span></span> | <span data-ttu-id="feb19-124">IDs de função em escopo de política, a menos que explicitamente excluído ou `All` .</span><span class="sxs-lookup"><span data-stu-id="feb19-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="feb19-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="feb19-125">excludeRoles</span></span> | <span data-ttu-id="feb19-126">String collection</span><span class="sxs-lookup"><span data-stu-id="feb19-126">String collection</span></span> | <span data-ttu-id="feb19-127">IDs de função excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="feb19-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="feb19-128">Relações</span><span class="sxs-lookup"><span data-stu-id="feb19-128">Relationships</span></span>

<span data-ttu-id="feb19-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feb19-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="feb19-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feb19-130">JSON representation</span></span>

<span data-ttu-id="feb19-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feb19-131">The following is a JSON representation of the resource.</span></span>

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
