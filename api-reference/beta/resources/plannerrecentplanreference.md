---
title: tipo de recurso plannerRecentPlanReference
description: 'O tipo de recurso **plannerRecentPlanReference** representa uma referência a um plannerPlan que foi recentemente exibido por um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9ef244c532264736c2f0e3e531d61964ca5b578a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344351"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="0ae8d-103">tipo de recurso plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="0ae8d-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ae8d-104">O tipo de recurso **plannerRecentPlanReference** representa uma referência a um [plannerPlan](plannerplan.md) que foi recentemente exibido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="0ae8d-105">O **plannerRecentPlanReferences** de um usuário é explicitamente mantido por aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="0ae8d-106">Qualquer aplicativo que implemente o recurso de planos recentes deve registrar quando o usuário tiver exibido o último plano e atualizar as entradas de **plannerRecentPlanReference** de acordo.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="0ae8d-107">Os aplicativos devem observar que as entradas do **plannerRecentPlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode mais acessar ou que foram atualizadas com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="0ae8d-108">Recomendamos que os aplicativos Notifiquem os usuários quando houver discrepâncias e mantenha as entradas atualizadas.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="0ae8d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ae8d-109">Properties</span></span>
| <span data-ttu-id="0ae8d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ae8d-110">Property</span></span>     | <span data-ttu-id="0ae8d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ae8d-111">Type</span></span>   |<span data-ttu-id="0ae8d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ae8d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ae8d-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ae8d-113">lastAccessedDateTime</span></span>|<span data-ttu-id="0ae8d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ae8d-114">DateTimeOffset</span></span>|<span data-ttu-id="0ae8d-115">A data e a hora em que o plano foi exibido pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="0ae8d-116">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0ae8d-117">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0ae8d-118">planTitle</span><span class="sxs-lookup"><span data-stu-id="0ae8d-118">planTitle</span></span>|<span data-ttu-id="0ae8d-119">String</span><span class="sxs-lookup"><span data-stu-id="0ae8d-119">String</span></span>|<span data-ttu-id="0ae8d-120">O título do plano no momento em que o usuário o exibiu.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ae8d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ae8d-121">JSON representation</span></span>

<span data-ttu-id="0ae8d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ae8d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
