---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: ad75f3a796f29f7f9c4497a3a15fd31dec0f1c6f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342265"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="a5080-102">Tipo de recurso MentionAction</span><span class="sxs-lookup"><span data-stu-id="a5080-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5080-103">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="a5080-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a5080-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5080-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a5080-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5080-106">Properties</span></span>

| <span data-ttu-id="a5080-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a5080-107">Property name</span></span> | <span data-ttu-id="a5080-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5080-108">Type</span></span>                       | <span data-ttu-id="a5080-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5080-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="a5080-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="a5080-110">mentionees</span></span>    | <span data-ttu-id="a5080-111">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a5080-111">[identitySet][] collection</span></span> | <span data-ttu-id="a5080-112">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="a5080-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="a5080-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="a5080-114">Remarks</span></span>

<span data-ttu-id="a5080-115">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a5080-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
