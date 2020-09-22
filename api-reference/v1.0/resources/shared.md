---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Compartilhados
localization_priority: Normal
description: O recurso Shared indica que um DriveItem foi compartilhado com outras pessoas.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9058b1e3f5f8dd77c22ee253746c7eba8c1df7c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009181"
---
# <a name="shared-resource-type"></a><span data-ttu-id="82d9c-103">Tipo de recurso Shared</span><span class="sxs-lookup"><span data-stu-id="82d9c-103">Shared resource type</span></span>

<span data-ttu-id="82d9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82d9c-p101">O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="82d9c-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="82d9c-107">Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.</span><span class="sxs-lookup"><span data-stu-id="82d9c-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82d9c-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82d9c-108">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="82d9c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82d9c-109">Properties</span></span>

| <span data-ttu-id="82d9c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82d9c-110">Property</span></span>       | <span data-ttu-id="82d9c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="82d9c-111">Type</span></span>                          | <span data-ttu-id="82d9c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="82d9c-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="82d9c-113">owner</span><span class="sxs-lookup"><span data-stu-id="82d9c-113">owner</span></span>          | [<span data-ttu-id="82d9c-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="82d9c-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="82d9c-p102">A identidade do proprietário do item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82d9c-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="82d9c-117">escopo</span><span class="sxs-lookup"><span data-stu-id="82d9c-117">scope</span></span>          | <span data-ttu-id="82d9c-118">String</span><span class="sxs-lookup"><span data-stu-id="82d9c-118">String</span></span>                        | <span data-ttu-id="82d9c-p103">Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82d9c-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="82d9c-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="82d9c-121">sharedBy</span></span>       | [<span data-ttu-id="82d9c-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="82d9c-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="82d9c-p104">A identidade do usuário que compartilhou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82d9c-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="82d9c-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="82d9c-125">sharedDateTime</span></span> | <span data-ttu-id="82d9c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82d9c-126">DateTimeOffset</span></span>                | <span data-ttu-id="82d9c-p105">A data e a hora UTC que o item foi compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82d9c-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="82d9c-129">Opções de escopo</span><span class="sxs-lookup"><span data-stu-id="82d9c-129">Scope options</span></span>

| <span data-ttu-id="82d9c-130">Valor</span><span class="sxs-lookup"><span data-stu-id="82d9c-130">Value</span></span>          | <span data-ttu-id="82d9c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="82d9c-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="82d9c-132">O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.</span><span class="sxs-lookup"><span data-stu-id="82d9c-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="82d9c-133">O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="82d9c-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="82d9c-134">O item é compartilhado apenas com usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="82d9c-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="82d9c-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="82d9c-135">Remarks</span></span>

<span data-ttu-id="82d9c-136">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="82d9c-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/shared.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization,users) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Shared"
} -->

