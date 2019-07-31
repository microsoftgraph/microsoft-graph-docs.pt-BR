---
author: daspek
description: O recurso ShareAction fornece informações sobre uma activity que compartilhou um item.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 10eb5b870a5ecd80f4a064d1dca496f216bf241d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965163"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="f3883-103">Tipo de recurso ShareAction</span><span class="sxs-lookup"><span data-stu-id="f3883-103">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3883-104">O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="f3883-104">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f3883-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3883-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f3883-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3883-106">Properties</span></span>

| <span data-ttu-id="f3883-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f3883-107">Property name</span></span> | <span data-ttu-id="f3883-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3883-108">Type</span></span>                       | <span data-ttu-id="f3883-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3883-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="f3883-110">recipients</span><span class="sxs-lookup"><span data-stu-id="f3883-110">recipients</span></span>    | <span data-ttu-id="f3883-111">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f3883-111">[identitySet][] collection</span></span> | <span data-ttu-id="f3883-112">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="f3883-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="f3883-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="f3883-114">Remarks</span></span>

<span data-ttu-id="f3883-115">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f3883-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
