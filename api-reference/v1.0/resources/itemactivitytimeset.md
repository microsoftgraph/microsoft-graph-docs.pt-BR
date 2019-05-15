---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActivityTimeSet
description: O objeto doactionset fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4ef0b56471afe78b13edc2f6efb25941c9a749df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970616"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="683c2-103">tipo de recurso itemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="683c2-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="683c2-104">O recurso **itemActivityTimeSet** fornece informações sobre quando uma [atividade] [ activity] em um item ocorreu.</span><span class="sxs-lookup"><span data-stu-id="683c2-104">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="683c2-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="683c2-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="683c2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="683c2-106">Properties</span></span>

| <span data-ttu-id="683c2-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="683c2-107">Property name</span></span>    | <span data-ttu-id="683c2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="683c2-108">Type</span></span>           | <span data-ttu-id="683c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="683c2-109">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="683c2-110">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="683c2-110">observedDateTime</span></span> | <span data-ttu-id="683c2-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="683c2-111">DateTimeOffset</span></span> | <span data-ttu-id="683c2-112">Quando observamos a atividade ocorrer.</span><span class="sxs-lookup"><span data-stu-id="683c2-112">When the activity was observed to take place.</span></span>
| <span data-ttu-id="683c2-113">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="683c2-113">recordedDateTime</span></span> | <span data-ttu-id="683c2-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="683c2-114">DateTimeOffset</span></span> | <span data-ttu-id="683c2-115">Quando a observação foi gravada no serviço.</span><span class="sxs-lookup"><span data-stu-id="683c2-115">When the observation was recorded on the service.</span></span>

<span data-ttu-id="683c2-116">A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.</span><span class="sxs-lookup"><span data-stu-id="683c2-116">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="683c2-117">Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="683c2-117">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="683c2-118">Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="683c2-118">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="683c2-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="683c2-119">JSON representation</span></span>

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
