---
author: daspek
description: O recurso ShareAction fornece informações sobre uma activity que compartilhou um item.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6d855b4c42a51e6ff9c9330f0a22e8076778d456
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010189"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="ac365-103">Tipo de recurso ShareAction</span><span class="sxs-lookup"><span data-stu-id="ac365-103">ShareAction resource type</span></span>

<span data-ttu-id="ac365-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac365-105">O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="ac365-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="ac365-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac365-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ac365-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac365-107">Properties</span></span>

| <span data-ttu-id="ac365-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ac365-108">Property name</span></span> | <span data-ttu-id="ac365-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac365-109">Type</span></span>                       | <span data-ttu-id="ac365-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac365-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="ac365-111">destinatários</span><span class="sxs-lookup"><span data-stu-id="ac365-111">recipients</span></span>    | <span data-ttu-id="ac365-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ac365-112">[identitySet][] collection</span></span> | <span data-ttu-id="ac365-113">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="ac365-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="ac365-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac365-115">Remarks</span></span>

<span data-ttu-id="ac365-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="ac365-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


