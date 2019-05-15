---
author: daspek
ms.author: dspektor
title: tipo de recurso shareaction
description: O objeto shareaction fornece informações sobre quem um item foi compartilhado em uma ação de compartilhamento.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a61ec47aae94eb99c2a192c863127d18a80fc087
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970592"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="d7c5c-103">tipo de recurso shareaction</span><span class="sxs-lookup"><span data-stu-id="d7c5c-103">shareAction resource type</span></span>

<span data-ttu-id="d7c5c-104">O \*\*\*\* recurso shareaction fornece informações sobre uma [atividade] [ activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="d7c5c-104">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="d7c5c-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d7c5c-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="d7c5c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7c5c-106">Properties</span></span>

| <span data-ttu-id="d7c5c-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d7c5c-107">Property name</span></span> | <span data-ttu-id="d7c5c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7c5c-108">Type</span></span>                       | <span data-ttu-id="d7c5c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7c5c-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="d7c5c-110">recipients</span><span class="sxs-lookup"><span data-stu-id="d7c5c-110">recipients</span></span>    | <span data-ttu-id="d7c5c-111">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d7c5c-111">[identitySet][] collection</span></span> | <span data-ttu-id="d7c5c-112">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="d7c5c-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="d7c5c-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7c5c-114">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->
