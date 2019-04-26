---
title: tipo de recurso plannerPlanContext
description: O recurso **plannerPlanContext** representa a relação de um plannerPlan com uma experiência de usuário fora do Planner. Os planos no Planner podem ser reproduzidos em outras experiências, como o Microsoft Teams, para controlar o trabalho no contexto da experiência.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 68d9233d2645c2176ad364fbcbfac869976f0586
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344442"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="cfb7e-104">tipo de recurso plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="cfb7e-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfb7e-105">O recurso **plannerPlanContext** representa a relação de um [plannerPlan](plannerplan.md) com uma experiência de usuário fora do Planner.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="cfb7e-106">Os planos no Planner podem ser reproduzidos em outras experiências, como o Microsoft Teams, para controlar o trabalho no contexto da experiência.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="cfb7e-107">A experiência que a entrada **plannerPlanContext** reenviado pode ser identificada com base na propriedade **ownerAppId** :</span><span class="sxs-lookup"><span data-stu-id="cfb7e-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="cfb7e-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: a entrada de contexto pertence ao Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="cfb7e-109">00000003-0000-0ff1-ce00-000000000000: a entrada de contexto pertence ao SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="cfb7e-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfb7e-110">Properties</span></span>
| <span data-ttu-id="cfb7e-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfb7e-111">Property</span></span>     | <span data-ttu-id="cfb7e-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfb7e-112">Type</span></span>   |<span data-ttu-id="cfb7e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb7e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfb7e-114">Association</span><span class="sxs-lookup"><span data-stu-id="cfb7e-114">associationType</span></span>|<span data-ttu-id="cfb7e-115">String</span><span class="sxs-lookup"><span data-stu-id="cfb7e-115">String</span></span>|<span data-ttu-id="cfb7e-116">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-116">Nullable.</span></span> <span data-ttu-id="cfb7e-117">Um tipo de associação definido pelo aplicativo entre o [plannerPlan](plannerplan.md) e o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="cfb7e-118">O aplicativo pode usar essas informações para rastrear diferentes tipos de relações com o mesmo [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="cfb7e-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="cfb7e-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfb7e-119">createdDateTime</span></span>|<span data-ttu-id="cfb7e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfb7e-120">DateTimeOffset</span></span>|<span data-ttu-id="cfb7e-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-121">Read-only.</span></span> <span data-ttu-id="cfb7e-122">A data e hora em que o **plannerPlanContext** foi criado.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="cfb7e-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cfb7e-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cfb7e-125">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="cfb7e-125">displayNameSegments</span></span>|<span data-ttu-id="cfb7e-126">Coleção String</span><span class="sxs-lookup"><span data-stu-id="cfb7e-126">String collection</span></span>|<span data-ttu-id="cfb7e-127">Os segmentos do nome da experiência externa.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="cfb7e-128">Segmentos representam uma estrutura hierárquica que permite que outros aplicativos exibam a relação.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="cfb7e-129">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="cfb7e-129">ownerAppId</span></span>|<span data-ttu-id="cfb7e-130">String</span><span class="sxs-lookup"><span data-stu-id="cfb7e-130">String</span></span>|<span data-ttu-id="cfb7e-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-131">Read-only.</span></span> <span data-ttu-id="cfb7e-132">ID do aplicativo que criou o **plannerPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfb7e-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfb7e-133">JSON representation</span></span>

<span data-ttu-id="cfb7e-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-134">The following is a JSON representation of the resource.</span></span>

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
