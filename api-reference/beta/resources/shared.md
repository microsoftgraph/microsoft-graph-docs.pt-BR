---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Compartilhados
ms.openlocfilehash: 38bc8604ba2528a24e2193a2fb521428b2b5c2d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038886"
---
# <a name="shared-resource-type"></a><span data-ttu-id="3eae5-102">Tipo de recurso Shared</span><span class="sxs-lookup"><span data-stu-id="3eae5-102">Shared resource type</span></span>

> <span data-ttu-id="3eae5-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3eae5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eae5-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3eae5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3eae5-p102">O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="3eae5-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="3eae5-107">Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.</span><span class="sxs-lookup"><span data-stu-id="3eae5-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3eae5-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3eae5-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3eae5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3eae5-109">Properties</span></span>

| <span data-ttu-id="3eae5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3eae5-110">Property</span></span>       | <span data-ttu-id="3eae5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eae5-111">Type</span></span>                          | <span data-ttu-id="3eae5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eae5-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="3eae5-113">owner</span><span class="sxs-lookup"><span data-stu-id="3eae5-113">owner</span></span>          | [<span data-ttu-id="3eae5-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3eae5-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="3eae5-p103">A identidade do proprietário do item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eae5-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="3eae5-117">scope</span><span class="sxs-lookup"><span data-stu-id="3eae5-117">scope</span></span>          | <span data-ttu-id="3eae5-118">String</span><span class="sxs-lookup"><span data-stu-id="3eae5-118">String</span></span>                        | <span data-ttu-id="3eae5-p104">Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eae5-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="3eae5-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="3eae5-121">sharedBy</span></span>       | [<span data-ttu-id="3eae5-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="3eae5-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="3eae5-p105">A identidade do usuário que compartilhou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eae5-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="3eae5-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="3eae5-125">sharedDateTime</span></span> | <span data-ttu-id="3eae5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eae5-126">DateTimeOffset</span></span>                | <span data-ttu-id="3eae5-p106">A data e a hora UTC que o item foi compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eae5-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="3eae5-129">Valores de escopo</span><span class="sxs-lookup"><span data-stu-id="3eae5-129">Scope values</span></span>

| <span data-ttu-id="3eae5-130">Valor</span><span class="sxs-lookup"><span data-stu-id="3eae5-130">Value</span></span>          | <span data-ttu-id="3eae5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eae5-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="3eae5-132">O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.</span><span class="sxs-lookup"><span data-stu-id="3eae5-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="3eae5-133">O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="3eae5-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="3eae5-134">O item é compartilhado apenas com usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="3eae5-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="3eae5-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="3eae5-135">Remarks</span></span>

<span data-ttu-id="3eae5-136">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3eae5-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
