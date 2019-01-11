---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Compartilhados
localization_priority: Normal
ms.openlocfilehash: cae69a60691d388570d29176fc20aac429907f8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838987"
---
# <a name="shared-resource-type"></a><span data-ttu-id="d3bff-102">Tipo de recurso Shared</span><span class="sxs-lookup"><span data-stu-id="d3bff-102">Shared resource type</span></span>

> <span data-ttu-id="d3bff-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3bff-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3bff-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3bff-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3bff-p102">O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d3bff-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="d3bff-107">Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.</span><span class="sxs-lookup"><span data-stu-id="d3bff-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3bff-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3bff-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d3bff-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3bff-109">Properties</span></span>

| <span data-ttu-id="d3bff-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3bff-110">Property</span></span>       | <span data-ttu-id="d3bff-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3bff-111">Type</span></span>                          | <span data-ttu-id="d3bff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3bff-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="d3bff-113">owner</span><span class="sxs-lookup"><span data-stu-id="d3bff-113">owner</span></span>          | [<span data-ttu-id="d3bff-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d3bff-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="d3bff-p103">A identidade do proprietário do item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3bff-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="d3bff-117">escopo</span><span class="sxs-lookup"><span data-stu-id="d3bff-117">scope</span></span>          | <span data-ttu-id="d3bff-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3bff-118">String</span></span>                        | <span data-ttu-id="d3bff-p104">Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3bff-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="d3bff-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="d3bff-121">sharedBy</span></span>       | [<span data-ttu-id="d3bff-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="d3bff-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="d3bff-p105">A identidade do usuário que compartilhou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3bff-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="d3bff-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3bff-125">sharedDateTime</span></span> | <span data-ttu-id="d3bff-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3bff-126">DateTimeOffset</span></span>                | <span data-ttu-id="d3bff-p106">A data e a hora UTC que o item foi compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3bff-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="d3bff-129">Valores de escopo</span><span class="sxs-lookup"><span data-stu-id="d3bff-129">Scope values</span></span>

| <span data-ttu-id="d3bff-130">Valor</span><span class="sxs-lookup"><span data-stu-id="d3bff-130">Value</span></span>          | <span data-ttu-id="d3bff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3bff-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="d3bff-132">O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.</span><span class="sxs-lookup"><span data-stu-id="d3bff-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="d3bff-133">O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="d3bff-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="d3bff-134">O item é compartilhado apenas com usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="d3bff-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="d3bff-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="d3bff-135">Remarks</span></span>

<span data-ttu-id="d3bff-136">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3bff-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
