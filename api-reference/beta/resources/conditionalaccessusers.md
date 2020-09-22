---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1294551fd568b9f41072d3707d64a88d4b04edc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994229"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="518fb-103">tipo de recurso conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="518fb-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="518fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="518fb-105">Representa usuários, grupos e funções incluídos e excluídos do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="518fb-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="518fb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="518fb-106">Properties</span></span>

| <span data-ttu-id="518fb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="518fb-107">Property</span></span>     | <span data-ttu-id="518fb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="518fb-108">Type</span></span>        | <span data-ttu-id="518fb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="518fb-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="518fb-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="518fb-110">includeUsers</span></span> | <span data-ttu-id="518fb-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="518fb-111">String collection</span></span> | <span data-ttu-id="518fb-112">IDs de usuário em escopo de política, a menos que explicitamente excluído ou ou `None` `All` `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="518fb-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="518fb-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="518fb-113">excludeUsers</span></span> | <span data-ttu-id="518fb-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="518fb-114">String collection</span></span> | <span data-ttu-id="518fb-115">IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` .</span><span class="sxs-lookup"><span data-stu-id="518fb-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="518fb-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="518fb-116">includeGroups</span></span> | <span data-ttu-id="518fb-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="518fb-117">String collection</span></span> | <span data-ttu-id="518fb-118">IDs de grupo em escopo de política, a menos que explicitamente excluído ou `All` .</span><span class="sxs-lookup"><span data-stu-id="518fb-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="518fb-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="518fb-119">excludeGroups</span></span> | <span data-ttu-id="518fb-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="518fb-120">String collection</span></span> | <span data-ttu-id="518fb-121">IDs de grupo excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="518fb-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="518fb-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="518fb-122">includeRoles</span></span> | <span data-ttu-id="518fb-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="518fb-123">String collection</span></span> | <span data-ttu-id="518fb-124">IDs de função em escopo de política, a menos que explicitamente excluído ou `All` .</span><span class="sxs-lookup"><span data-stu-id="518fb-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="518fb-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="518fb-125">excludeRoles</span></span> | <span data-ttu-id="518fb-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="518fb-126">String collection</span></span> | <span data-ttu-id="518fb-127">IDs de função excluídas do escopo da política.</span><span class="sxs-lookup"><span data-stu-id="518fb-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="518fb-128">Relações</span><span class="sxs-lookup"><span data-stu-id="518fb-128">Relationships</span></span>

<span data-ttu-id="518fb-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="518fb-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="518fb-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="518fb-130">JSON representation</span></span>

<span data-ttu-id="518fb-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="518fb-131">The following is a JSON representation of the resource.</span></span>

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

