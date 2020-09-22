---
title: tipo de recurso plannerPlanContext
description: O recurso **plannerPlanContext** representa a relação de um plannerPlan com uma experiência de usuário fora do Planner. Os planos no Planner podem ser reproduzidos em outras experiências, como o Microsoft Teams, para controlar o trabalho no contexto da experiência.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c1163843cdb393363bbb30783aa8232aa67544ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979334"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="97e30-104">tipo de recurso plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="97e30-104">plannerPlanContext resource type</span></span>

<span data-ttu-id="97e30-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97e30-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97e30-106">O recurso **plannerPlanContext** representa a relação de um [plannerPlan](plannerplan.md) com uma experiência de usuário fora do Planner.</span><span class="sxs-lookup"><span data-stu-id="97e30-106">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="97e30-107">Os planos no Planner podem ser reproduzidos em outras experiências, como o Microsoft Teams, para controlar o trabalho no contexto da experiência.</span><span class="sxs-lookup"><span data-stu-id="97e30-107">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="97e30-108">A experiência que a entrada **plannerPlanContext** reenviado pode ser identificada com base na propriedade **ownerAppId** :</span><span class="sxs-lookup"><span data-stu-id="97e30-108">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
- <span data-ttu-id="97e30-109">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: a entrada de contexto pertence ao Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="97e30-109">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
- <span data-ttu-id="97e30-110">00000003-0000-0ff1-ce00-000000000000: a entrada de contexto pertence ao SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97e30-110">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="97e30-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97e30-111">Properties</span></span>
| <span data-ttu-id="97e30-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97e30-112">Property</span></span>     | <span data-ttu-id="97e30-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e30-113">Type</span></span>   |<span data-ttu-id="97e30-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e30-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97e30-115">Association</span><span class="sxs-lookup"><span data-stu-id="97e30-115">associationType</span></span>|<span data-ttu-id="97e30-116">String</span><span class="sxs-lookup"><span data-stu-id="97e30-116">String</span></span>|<span data-ttu-id="97e30-117">Anulável.</span><span class="sxs-lookup"><span data-stu-id="97e30-117">Nullable.</span></span> <span data-ttu-id="97e30-118">Um tipo de associação definido pelo aplicativo entre o [plannerPlan](plannerplan.md) e o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97e30-118">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="97e30-119">O aplicativo pode usar essas informações para rastrear diferentes tipos de relações com o mesmo [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="97e30-119">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="97e30-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97e30-120">createdDateTime</span></span>|<span data-ttu-id="97e30-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e30-121">DateTimeOffset</span></span>|<span data-ttu-id="97e30-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97e30-122">Read-only.</span></span> <span data-ttu-id="97e30-123">A data e hora em que o **plannerPlanContext** foi criado.</span><span class="sxs-lookup"><span data-stu-id="97e30-123">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="97e30-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97e30-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97e30-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97e30-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="97e30-126">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="97e30-126">displayNameSegments</span></span>|<span data-ttu-id="97e30-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="97e30-127">String collection</span></span>|<span data-ttu-id="97e30-128">Os segmentos do nome da experiência externa.</span><span class="sxs-lookup"><span data-stu-id="97e30-128">The segments of the name of the external experience.</span></span> <span data-ttu-id="97e30-129">Segmentos representam uma estrutura hierárquica que permite que outros aplicativos exibam a relação.</span><span class="sxs-lookup"><span data-stu-id="97e30-129">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="97e30-130">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="97e30-130">ownerAppId</span></span>|<span data-ttu-id="97e30-131">String</span><span class="sxs-lookup"><span data-stu-id="97e30-131">String</span></span>|<span data-ttu-id="97e30-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97e30-132">Read-only.</span></span> <span data-ttu-id="97e30-133">ID do aplicativo que criou o **plannerPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="97e30-133">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97e30-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97e30-134">JSON representation</span></span>

<span data-ttu-id="97e30-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97e30-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


