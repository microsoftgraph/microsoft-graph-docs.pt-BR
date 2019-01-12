---
title: tipo de recurso de plannerRecentPlanReference
description: 'O recurso de **plannerRecentPlanReference** digite representa uma referência a um plannerPlan que recentemente foi exibido por um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bafaf6d20dc8f64ffe49eb4e2f998607708a2773
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943522"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="093c8-103">tipo de recurso de plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="093c8-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="093c8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="093c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="093c8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="093c8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="093c8-106">O recurso de **plannerRecentPlanReference** digite representa uma referência a um [plannerPlan](plannerplan.md) recentemente foi exibido por um usuário.</span><span class="sxs-lookup"><span data-stu-id="093c8-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="093c8-107">O **plannerRecentPlanReferences** para um usuário explicitamente são mantidas por aplicativos.</span><span class="sxs-lookup"><span data-stu-id="093c8-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="093c8-108">Qualquer aplicativo que implementa o recurso de planos recente deve gravar quando o usuário visualizado por último entradas de **plannerRecentPlanReference** de atualização e um plano de acordo.</span><span class="sxs-lookup"><span data-stu-id="093c8-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="093c8-109">Aplicativos Lembre-se de que as entradas de **plannerRecentPlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode acessar ou que foram atualizados com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="093c8-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="093c8-110">É recomendável que os aplicativos notificar os usuários quando houver discrepâncias e manter as entradas atualizado.</span><span class="sxs-lookup"><span data-stu-id="093c8-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="093c8-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="093c8-111">Properties</span></span>
| <span data-ttu-id="093c8-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="093c8-112">Property</span></span>     | <span data-ttu-id="093c8-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="093c8-113">Type</span></span>   |<span data-ttu-id="093c8-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="093c8-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="093c8-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="093c8-115">lastAccessedDateTime</span></span>|<span data-ttu-id="093c8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="093c8-116">DateTimeOffset</span></span>|<span data-ttu-id="093c8-117">A data e hora que o plano foi visualizado por último pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="093c8-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="093c8-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="093c8-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="093c8-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="093c8-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="093c8-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="093c8-120">planTitle</span></span>|<span data-ttu-id="093c8-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="093c8-121">String</span></span>|<span data-ttu-id="093c8-122">O título do plano no momento em que o usuário exibidos-lo.</span><span class="sxs-lookup"><span data-stu-id="093c8-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="093c8-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="093c8-123">JSON representation</span></span>

<span data-ttu-id="093c8-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="093c8-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
