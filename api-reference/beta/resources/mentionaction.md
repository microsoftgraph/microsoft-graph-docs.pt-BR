---
author: daspek
description: O recurso MentionAction fornece informações sobre um atividade que mencionou pessoas.
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: b0f8376c3fcc86cdd16c1eeb32507e5b26469285
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971598"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="7ac1e-103">Tipo de recurso MentionAction</span><span class="sxs-lookup"><span data-stu-id="7ac1e-103">MentionAction resource type</span></span>

<span data-ttu-id="7ac1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac1e-105">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="7ac1e-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7ac1e-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ac1e-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="7ac1e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ac1e-108">Properties</span></span>

| <span data-ttu-id="7ac1e-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac1e-109">Property name</span></span> | <span data-ttu-id="7ac1e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac1e-110">Type</span></span>                       | <span data-ttu-id="7ac1e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac1e-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="7ac1e-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="7ac1e-112">mentionees</span></span>    | <span data-ttu-id="7ac1e-113">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7ac1e-113">[identitySet][] collection</span></span> | <span data-ttu-id="7ac1e-114">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="7ac1e-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="7ac1e-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="7ac1e-116">Remarks</span></span>

<span data-ttu-id="7ac1e-117">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="7ac1e-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->


