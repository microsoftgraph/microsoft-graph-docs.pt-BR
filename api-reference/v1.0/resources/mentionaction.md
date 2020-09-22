---
author: daspek
ms.author: dspektor
title: tipo de recurso mençãoaction
description: O objeto Mençãoaction fornece informações sobre quem foi mencionado durante uma atividade.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8937a8f7acd55af93fdeac9eceb17d46e2cf495c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991898"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="4f382-103">tipo de recurso mençãoaction</span><span class="sxs-lookup"><span data-stu-id="4f382-103">mentionAction resource type</span></span>

<span data-ttu-id="4f382-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f382-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f382-105">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="4f382-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="4f382-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4f382-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="4f382-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f382-108">Properties</span></span>

| <span data-ttu-id="4f382-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4f382-109">Property name</span></span> | <span data-ttu-id="4f382-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f382-110">Type</span></span>                       | <span data-ttu-id="4f382-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f382-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="4f382-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="4f382-112">mentionees</span></span>    | <span data-ttu-id="4f382-113">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4f382-113">[identitySet][] collection</span></span> | <span data-ttu-id="4f382-114">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="4f382-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="4f382-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f382-116">JSON representation</span></span>

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

