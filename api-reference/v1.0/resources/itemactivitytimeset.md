---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActivityTimeSet
description: O objeto doactionset fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9dce21afc1acc8e93181204e026f74a597c9120f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036586"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="4cbf3-103">tipo de recurso itemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="4cbf3-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="4cbf3-104">O recurso **itemActivityTimeSet** fornece informações sobre quando uma [atividade][activity] em um item ocorreu.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-104">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="4cbf3-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="4cbf3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cbf3-106">Properties</span></span>

| <span data-ttu-id="4cbf3-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4cbf3-107">Property name</span></span>    | <span data-ttu-id="4cbf3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cbf3-108">Type</span></span>           | <span data-ttu-id="4cbf3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cbf3-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="4cbf3-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cbf3-110">observedDateTime</span></span> | <span data-ttu-id="4cbf3-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cbf3-111">DateTimeOffset</span></span> | <span data-ttu-id="4cbf3-112">Quando observamos a atividade ocorrer.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="4cbf3-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cbf3-113">recordedDateTime</span></span> | <span data-ttu-id="4cbf3-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cbf3-114">DateTimeOffset</span></span> | <span data-ttu-id="4cbf3-115">Quando a observação foi gravada no serviço.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="4cbf3-116">A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="4cbf3-117">Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="4cbf3-118">Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="4cbf3-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cbf3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cbf3-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
