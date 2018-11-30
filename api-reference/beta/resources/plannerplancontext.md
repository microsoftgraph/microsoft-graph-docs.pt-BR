---
title: tipo de recurso de plannerPlanContext
description: O recurso de **plannerPlanContext** representa a relação entre um plannerPlan a uma experiência de usuário fora do planejador. Planos no planejador podem ser exibidos em outras experiências, como Teams da Microsoft, para controlar o trabalho no contexto dessa experiência.
ms.openlocfilehash: 84512c03081a3e1fd2b15456c64cecf3f9c39435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037297"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="83fe7-104">tipo de recurso de plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="83fe7-104">plannerPlanContext resource type</span></span>

> <span data-ttu-id="83fe7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="83fe7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83fe7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="83fe7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83fe7-107">O recurso de **plannerPlanContext** representa a relação entre um [plannerPlan](plannerplan.md) a uma experiência de usuário fora do planejador.</span><span class="sxs-lookup"><span data-stu-id="83fe7-107">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="83fe7-108">Planos no planejador podem ser exibidos em outras experiências, como Teams da Microsoft, para controlar o trabalho no contexto dessa experiência.</span><span class="sxs-lookup"><span data-stu-id="83fe7-108">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="83fe7-109">A experiência que a entrada **plannerPlanContext** reresents pode ser identificada com base na propriedade **ownerAppId** :</span><span class="sxs-lookup"><span data-stu-id="83fe7-109">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="83fe7-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: A entrada do contexto pertence à Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="83fe7-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="83fe7-111">00000003-0000-0ff1-CE00-000000000000: pertence a entrada do contexto do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="83fe7-111">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="83fe7-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83fe7-112">Properties</span></span>
| <span data-ttu-id="83fe7-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83fe7-113">Property</span></span>     | <span data-ttu-id="83fe7-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="83fe7-114">Type</span></span>   |<span data-ttu-id="83fe7-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="83fe7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83fe7-116">associationType</span><span class="sxs-lookup"><span data-stu-id="83fe7-116">associationType</span></span>|<span data-ttu-id="83fe7-117">String</span><span class="sxs-lookup"><span data-stu-id="83fe7-117">String</span></span>|<span data-ttu-id="83fe7-118">Anulável.</span><span class="sxs-lookup"><span data-stu-id="83fe7-118">Nullable.</span></span> <span data-ttu-id="83fe7-119">Um tipo definido pelo aplicativo de associação entre o [plannerPlan](plannerplan.md) e o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="83fe7-119">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="83fe7-120">O aplicativo pode usar essas informações para rastrear diferentes tipos de relacionamentos para o mesmo [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="83fe7-120">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="83fe7-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83fe7-121">createdDateTime</span></span>|<span data-ttu-id="83fe7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83fe7-122">DateTimeOffset</span></span>|<span data-ttu-id="83fe7-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83fe7-123">Read-only.</span></span> <span data-ttu-id="83fe7-124">A data e hora em que o **plannerPlanContext** foi criado.</span><span class="sxs-lookup"><span data-stu-id="83fe7-124">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="83fe7-125">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="83fe7-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="83fe7-126">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="83fe7-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="83fe7-127">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="83fe7-127">displayNameSegments</span></span>|<span data-ttu-id="83fe7-128">String collection</span><span class="sxs-lookup"><span data-stu-id="83fe7-128">String collection</span></span>|<span data-ttu-id="83fe7-129">Os segmentos do nome da experiência do externo.</span><span class="sxs-lookup"><span data-stu-id="83fe7-129">The segments of the name of the external experience.</span></span> <span data-ttu-id="83fe7-130">Segmentos representam uma estrutura hierárquica que permite a outros aplicativos exibir o relacionamento.</span><span class="sxs-lookup"><span data-stu-id="83fe7-130">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="83fe7-131">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="83fe7-131">ownerAppId</span></span>|<span data-ttu-id="83fe7-132">String</span><span class="sxs-lookup"><span data-stu-id="83fe7-132">String</span></span>|<span data-ttu-id="83fe7-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83fe7-133">Read-only.</span></span> <span data-ttu-id="83fe7-134">ID do aplicativo que criou o **plannerPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="83fe7-134">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83fe7-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83fe7-135">JSON representation</span></span>

<span data-ttu-id="83fe7-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83fe7-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
