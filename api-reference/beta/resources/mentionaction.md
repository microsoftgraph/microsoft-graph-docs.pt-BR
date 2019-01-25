---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9101ffed094fd78189b73eab511be88c8bf449de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513008"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="1d9ad-102">Tipo de recurso MentionAction</span><span class="sxs-lookup"><span data-stu-id="1d9ad-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d9ad-103">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="1d9ad-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1d9ad-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d9ad-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1d9ad-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d9ad-106">Properties</span></span>

| <span data-ttu-id="1d9ad-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1d9ad-107">Property name</span></span> | <span data-ttu-id="1d9ad-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d9ad-108">Type</span></span>                       | <span data-ttu-id="1d9ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d9ad-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="1d9ad-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="1d9ad-110">mentionees</span></span>    | <span data-ttu-id="1d9ad-111">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1d9ad-111">[identitySet][] collection</span></span> | <span data-ttu-id="1d9ad-112">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="1d9ad-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="1d9ad-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="1d9ad-114">Remarks</span></span>

<span data-ttu-id="1d9ad-115">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1d9ad-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
