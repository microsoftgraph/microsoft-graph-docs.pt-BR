---
author: daspek
title: Tipo de recurso itemActivityTimeSet
description: O objeto itemActionSet fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1f614c597efdb95b04c4079bd68240aa865d66dd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238670"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="a2212-103">Tipo de recurso itemActivityTimeSet</span><span class="sxs-lookup"><span data-stu-id="a2212-103">itemActivityTimeSet resource type</span></span>

<span data-ttu-id="a2212-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2212-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2212-105">O **recurso itemActivityTimeSet** fornece informações sobre quando [ocorreu uma atividade][activity] em um item.</span><span class="sxs-lookup"><span data-stu-id="a2212-105">The **itemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

><span data-ttu-id="a2212-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a2212-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="a2212-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2212-107">Properties</span></span>

| <span data-ttu-id="a2212-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a2212-108">Property name</span></span>    | <span data-ttu-id="a2212-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2212-109">Type</span></span>           | <span data-ttu-id="a2212-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2212-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="a2212-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2212-111">observedDateTime</span></span> | <span data-ttu-id="a2212-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2212-112">DateTimeOffset</span></span> | <span data-ttu-id="a2212-113">Quando observamos a atividade ocorrer.</span><span class="sxs-lookup"><span data-stu-id="a2212-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="a2212-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2212-114">recordedDateTime</span></span> | <span data-ttu-id="a2212-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2212-115">DateTimeOffset</span></span> | <span data-ttu-id="a2212-116">Quando a observação foi gravada no serviço.</span><span class="sxs-lookup"><span data-stu-id="a2212-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="a2212-117">A diferença entre os tempos de **observado** e **gravado** é particularmente importante para cenários de colaboração offline.</span><span class="sxs-lookup"><span data-stu-id="a2212-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="a2212-118">Se um usuário comenta em um arquivo enquanto está offline, o tempo pelo qual eles fazem o comentário é definido como o **observedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="a2212-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="a2212-119">Em um momento posterior quando o usuário se conectar novamente à nuvem e as alterações forem carregadas, esse momento posterior será definido como o **recordedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="a2212-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2212-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2212-120">JSON representation</span></span>

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

