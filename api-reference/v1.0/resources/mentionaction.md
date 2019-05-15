---
author: daspek
ms.author: dspektor
title: tipo de recurso mençãoaction
description: O objeto Mençãoaction fornece informações sobre quem foi mencionado durante uma atividade.
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8c09de2a36be2cd83d5e33cf2ed948c25819fe4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970618"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="ae408-103">tipo de recurso mençãoaction</span><span class="sxs-lookup"><span data-stu-id="ae408-103">mentionAction resource type</span></span>

<span data-ttu-id="ae408-104">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="ae408-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="ae408-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="ae408-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="ae408-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae408-107">Properties</span></span>

| <span data-ttu-id="ae408-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ae408-108">Property name</span></span> | <span data-ttu-id="ae408-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae408-109">Type</span></span>                       | <span data-ttu-id="ae408-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae408-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="ae408-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="ae408-111">mentionees</span></span>    | <span data-ttu-id="ae408-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ae408-112">[identitySet][] collection</span></span> | <span data-ttu-id="ae408-113">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="ae408-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="ae408-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae408-115">JSON representation</span></span>

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
