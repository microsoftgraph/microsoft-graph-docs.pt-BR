---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Compartilhados
localization_priority: Normal
ms.openlocfilehash: 04504b5257dfc49ad14cbee1f645120dc31a3387
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584076"
---
# <a name="shared-resource-type"></a><span data-ttu-id="a33f7-102">Tipo de recurso Shared</span><span class="sxs-lookup"><span data-stu-id="a33f7-102">Shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a33f7-p101">O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a33f7-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="a33f7-105">Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.</span><span class="sxs-lookup"><span data-stu-id="a33f7-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a33f7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a33f7-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a33f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a33f7-107">Properties</span></span>

| <span data-ttu-id="a33f7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a33f7-108">Property</span></span>       | <span data-ttu-id="a33f7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a33f7-109">Type</span></span>                          | <span data-ttu-id="a33f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a33f7-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="a33f7-111">owner</span><span class="sxs-lookup"><span data-stu-id="a33f7-111">owner</span></span>          | [<span data-ttu-id="a33f7-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="a33f7-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="a33f7-p102">A identidade do proprietário do item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a33f7-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="a33f7-115">escopo</span><span class="sxs-lookup"><span data-stu-id="a33f7-115">scope</span></span>          | <span data-ttu-id="a33f7-116">String</span><span class="sxs-lookup"><span data-stu-id="a33f7-116">String</span></span>                        | <span data-ttu-id="a33f7-p103">Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a33f7-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="a33f7-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="a33f7-119">sharedBy</span></span>       | [<span data-ttu-id="a33f7-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="a33f7-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="a33f7-p104">A identidade do usuário que compartilhou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a33f7-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="a33f7-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="a33f7-123">sharedDateTime</span></span> | <span data-ttu-id="a33f7-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a33f7-124">DateTimeOffset</span></span>                | <span data-ttu-id="a33f7-p105">A data e a hora UTC que o item foi compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a33f7-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="a33f7-127">Valores de escopo</span><span class="sxs-lookup"><span data-stu-id="a33f7-127">Scope values</span></span>

| <span data-ttu-id="a33f7-128">Valor</span><span class="sxs-lookup"><span data-stu-id="a33f7-128">Value</span></span>          | <span data-ttu-id="a33f7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a33f7-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="a33f7-130">O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.</span><span class="sxs-lookup"><span data-stu-id="a33f7-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="a33f7-131">O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="a33f7-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="a33f7-132">O item é compartilhado apenas com usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="a33f7-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="a33f7-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="a33f7-133">Remarks</span></span>

<span data-ttu-id="a33f7-134">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a33f7-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": [
    "Error: /api-reference/beta/resources/shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
