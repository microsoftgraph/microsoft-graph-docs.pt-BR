---
author: daspek
title: Tipo de recurso mentionAction
description: O objeto MentionAction fornece informações sobre quem foi mencionado durante uma atividade.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bc876f05949beb09b3e495a8b9b0536070b352cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238383"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="49a6f-103">Tipo de recurso mentionAction</span><span class="sxs-lookup"><span data-stu-id="49a6f-103">mentionAction resource type</span></span>

<span data-ttu-id="49a6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49a6f-105">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="49a6f-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="49a6f-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="49a6f-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="49a6f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49a6f-108">Properties</span></span>

| <span data-ttu-id="49a6f-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="49a6f-109">Property name</span></span> | <span data-ttu-id="49a6f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="49a6f-110">Type</span></span>                       | <span data-ttu-id="49a6f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49a6f-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="49a6f-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="49a6f-112">mentionees</span></span>    | <span data-ttu-id="49a6f-113">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="49a6f-113">[identitySet][] collection</span></span> | <span data-ttu-id="49a6f-114">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="49a6f-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="49a6f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49a6f-116">JSON representation</span></span>

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

