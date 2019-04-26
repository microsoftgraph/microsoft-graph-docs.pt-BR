---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 785a0a9ac9a2a1ecbd40c0d8ccae16dca9594fdf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584086"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="1cd12-102">Tipo de recurso ShareAction</span><span class="sxs-lookup"><span data-stu-id="1cd12-102">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cd12-103">O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="1cd12-103">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1cd12-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cd12-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="1cd12-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cd12-105">Properties</span></span>

| <span data-ttu-id="1cd12-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1cd12-106">Property name</span></span> | <span data-ttu-id="1cd12-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd12-107">Type</span></span>                       | <span data-ttu-id="1cd12-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd12-108">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="1cd12-109">recipients</span><span class="sxs-lookup"><span data-stu-id="1cd12-109">recipients</span></span>    | <span data-ttu-id="1cd12-110">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1cd12-110">[identitySet][] collection</span></span> | <span data-ttu-id="1cd12-111">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="1cd12-111">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="1cd12-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="1cd12-113">Remarks</span></span>

<span data-ttu-id="1cd12-114">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1cd12-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->
