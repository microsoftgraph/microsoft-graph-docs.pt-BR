---
author: daspek
description: O recurso ShareAction fornece informações sobre uma activity que compartilhou um item.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 94bf1b519308043f3421dc211eac006cfc4fd601
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520742"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="58d74-103">Tipo de recurso ShareAction</span><span class="sxs-lookup"><span data-stu-id="58d74-103">ShareAction resource type</span></span>

<span data-ttu-id="58d74-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="58d74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58d74-105">O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="58d74-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="58d74-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58d74-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="58d74-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58d74-107">Properties</span></span>

| <span data-ttu-id="58d74-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="58d74-108">Property name</span></span> | <span data-ttu-id="58d74-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="58d74-109">Type</span></span>                       | <span data-ttu-id="58d74-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d74-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="58d74-111">destinatários</span><span class="sxs-lookup"><span data-stu-id="58d74-111">recipients</span></span>    | <span data-ttu-id="58d74-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="58d74-112">[identitySet][] collection</span></span> | <span data-ttu-id="58d74-113">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="58d74-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="58d74-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="58d74-115">Remarks</span></span>

<span data-ttu-id="58d74-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="58d74-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
