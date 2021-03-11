---
title: Tipo de recurso plannerPlanContext
description: O **recurso plannerPlanContext** representa a relação de um plannerPlan para uma experiência de usuário fora do Planner. Os planos no Planner podem aparecer em outras experiências, como o Microsoft Teams, para acompanhar o trabalho no contexto dessa experiência.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8a3b82c35339bb8bc6b3d3d7923b41ed97ecc02
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720981"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="5c23a-104">Tipo de recurso plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="5c23a-104">plannerPlanContext resource type</span></span>

<span data-ttu-id="5c23a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c23a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c23a-106">O **recurso plannerPlanContext** representa a relação de um [plannerPlan](plannerplan.md) para uma experiência de usuário fora do Planner.</span><span class="sxs-lookup"><span data-stu-id="5c23a-106">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="5c23a-107">Os planos no Planner podem aparecer em outras experiências, como o Microsoft Teams, para acompanhar o trabalho no contexto dessa experiência.</span><span class="sxs-lookup"><span data-stu-id="5c23a-107">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span> <span data-ttu-id="5c23a-108">Experiências com links externos no [plannerPlanContextDetails](plannerplancontextdetails.md) podem ser exibidas em uma interface do usuário, permitindo que os usuários visite essas experiências.</span><span class="sxs-lookup"><span data-stu-id="5c23a-108">Experiences that have external links in the [plannerPlanContextDetails](plannerplancontextdetails.md) can be displayed in a user interface, allowing users to visit these experiences.</span></span>


## <a name="properties"></a><span data-ttu-id="5c23a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c23a-109">Properties</span></span>
| <span data-ttu-id="5c23a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c23a-110">Property</span></span>     | <span data-ttu-id="5c23a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c23a-111">Type</span></span>   |<span data-ttu-id="5c23a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c23a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c23a-113">associationType</span><span class="sxs-lookup"><span data-stu-id="5c23a-113">associationType</span></span>|<span data-ttu-id="5c23a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c23a-114">String</span></span>|<span data-ttu-id="5c23a-115">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5c23a-115">Nullable.</span></span> <span data-ttu-id="5c23a-116">Um tipo de associação definido pelo aplicativo entre o [plannerPlan](plannerplan.md) e o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c23a-116">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="5c23a-117">O aplicativo pode usar essas informações para rastrear diferentes tipos de relações com o mesmo [plannerPlan](plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="5c23a-117">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="5c23a-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c23a-118">createdDateTime</span></span>|<span data-ttu-id="5c23a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c23a-119">DateTimeOffset</span></span>|<span data-ttu-id="5c23a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c23a-120">Read-only.</span></span> <span data-ttu-id="5c23a-121">A data e a hora em que **o plannerPlanContext** foi criado.</span><span class="sxs-lookup"><span data-stu-id="5c23a-121">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="5c23a-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5c23a-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c23a-123">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5c23a-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5c23a-124">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="5c23a-124">displayNameSegments</span></span>|<span data-ttu-id="5c23a-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c23a-125">String collection</span></span>|<span data-ttu-id="5c23a-126">Os segmentos do nome da experiência externa.</span><span class="sxs-lookup"><span data-stu-id="5c23a-126">The segments of the name of the external experience.</span></span> <span data-ttu-id="5c23a-127">Os segmentos representam uma estrutura hierárquica que permite que outros aplicativos exibem a relação.</span><span class="sxs-lookup"><span data-stu-id="5c23a-127">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="5c23a-128">isCreationContext</span><span class="sxs-lookup"><span data-stu-id="5c23a-128">isCreationContext</span></span>|<span data-ttu-id="5c23a-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c23a-129">Boolean</span></span>|<span data-ttu-id="5c23a-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c23a-130">Read-only.</span></span> <span data-ttu-id="5c23a-131">Indica se o plano é criado a partir do contexto especificado.</span><span class="sxs-lookup"><span data-stu-id="5c23a-131">Indicates whether the plan is created from the specified context.</span></span> <span data-ttu-id="5c23a-132">Gerado automaticamente com base em se o contexto é especificado como parte da criação do plano.</span><span class="sxs-lookup"><span data-stu-id="5c23a-132">Auto-generated based on whether the context is specified as part of plan creation.</span></span>|
|<span data-ttu-id="5c23a-133">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="5c23a-133">ownerAppId</span></span>|<span data-ttu-id="5c23a-134">String</span><span class="sxs-lookup"><span data-stu-id="5c23a-134">String</span></span>|<span data-ttu-id="5c23a-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c23a-135">Read-only.</span></span> <span data-ttu-id="5c23a-136">ID do aplicativo que criou o **plannerPlanContext**.</span><span class="sxs-lookup"><span data-stu-id="5c23a-136">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c23a-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c23a-137">JSON representation</span></span>

<span data-ttu-id="5c23a-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c23a-138">The following is a JSON representation of the resource.</span></span>

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
  "isCreationContext": false,
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


