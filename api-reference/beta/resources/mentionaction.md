---
author: daspek
description: O recurso MentionAction fornece informações sobre um atividade que mencionou pessoas.
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1b08233569fe655b5a8f0e878c4e14d178be279f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966815"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="1923f-103">Tipo de recurso MentionAction</span><span class="sxs-lookup"><span data-stu-id="1923f-103">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1923f-104">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="1923f-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1923f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1923f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1923f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1923f-107">Properties</span></span>

| <span data-ttu-id="1923f-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1923f-108">Property name</span></span> | <span data-ttu-id="1923f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1923f-109">Type</span></span>                       | <span data-ttu-id="1923f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1923f-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="1923f-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="1923f-111">mentionees</span></span>    | <span data-ttu-id="1923f-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1923f-112">[identitySet][] collection</span></span> | <span data-ttu-id="1923f-113">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="1923f-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="1923f-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="1923f-115">Remarks</span></span>

<span data-ttu-id="1923f-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1923f-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
