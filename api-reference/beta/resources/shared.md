---
author: JeremyKelley
description: O recurso Shared indica que um DriveItem foi compartilhado com outras pessoas.
ms.date: 09/10/2017
title: Compartilhados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: dc867120028f1f36672f429ace0738779e9f9d48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973684"
---
# <a name="shared-resource-type"></a><span data-ttu-id="2c252-103">Tipo de recurso Shared</span><span class="sxs-lookup"><span data-stu-id="2c252-103">Shared resource type</span></span>

<span data-ttu-id="2c252-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c252-p101">O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2c252-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="2c252-107">Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.</span><span class="sxs-lookup"><span data-stu-id="2c252-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c252-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c252-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2c252-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c252-109">Properties</span></span>

| <span data-ttu-id="2c252-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c252-110">Property</span></span>       | <span data-ttu-id="2c252-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c252-111">Type</span></span>                          | <span data-ttu-id="2c252-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c252-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="2c252-113">owner</span><span class="sxs-lookup"><span data-stu-id="2c252-113">owner</span></span>          | [<span data-ttu-id="2c252-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2c252-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="2c252-p102">A identidade do proprietário do item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c252-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="2c252-117">escopo</span><span class="sxs-lookup"><span data-stu-id="2c252-117">scope</span></span>          | <span data-ttu-id="2c252-118">String</span><span class="sxs-lookup"><span data-stu-id="2c252-118">String</span></span>                        | <span data-ttu-id="2c252-p103">Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c252-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="2c252-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="2c252-121">sharedBy</span></span>       | [<span data-ttu-id="2c252-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="2c252-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="2c252-p104">A identidade do usuário que compartilhou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c252-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="2c252-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c252-125">sharedDateTime</span></span> | <span data-ttu-id="2c252-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c252-126">DateTimeOffset</span></span>                | <span data-ttu-id="2c252-p105">A data e a hora UTC que o item foi compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c252-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="2c252-129">Valores de escopo</span><span class="sxs-lookup"><span data-stu-id="2c252-129">Scope values</span></span>

| <span data-ttu-id="2c252-130">Valor</span><span class="sxs-lookup"><span data-stu-id="2c252-130">Value</span></span>          | <span data-ttu-id="2c252-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c252-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="2c252-132">O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.</span><span class="sxs-lookup"><span data-stu-id="2c252-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="2c252-133">O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="2c252-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="2c252-134">O item é compartilhado apenas com usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="2c252-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="2c252-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c252-135">Remarks</span></span>

<span data-ttu-id="2c252-136">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2c252-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": []
}
-->


