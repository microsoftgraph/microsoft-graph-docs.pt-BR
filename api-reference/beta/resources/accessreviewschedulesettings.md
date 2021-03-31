---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a uma série de revisão `accessReviewScheduleSettings` de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77ea7d8601df36525aad7a3448aa3b6f031d98d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469315"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="62a78-103">Tipo de recurso accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="62a78-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="62a78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="62a78-105">O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="62a78-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="62a78-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62a78-106">Properties</span></span>
| <span data-ttu-id="62a78-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62a78-107">Property</span></span>    | <span data-ttu-id="62a78-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62a78-108">Type</span></span>   | <span data-ttu-id="62a78-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a78-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="62a78-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="62a78-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="62a78-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="62a78-111">Boolean</span></span> | <span data-ttu-id="62a78-112">Sinalizador para indicar se os emails estão habilitados/desabilitados.</span><span class="sxs-lookup"><span data-stu-id="62a78-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="62a78-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="62a78-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="62a78-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="62a78-114">Boolean</span></span>  | <span data-ttu-id="62a78-115">Sinalizador para indicar se os lembretes estão habilitados/desabilitados.</span><span class="sxs-lookup"><span data-stu-id="62a78-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="62a78-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="62a78-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="62a78-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="62a78-117">Boolean</span></span> | <span data-ttu-id="62a78-118">Sinalizador para indicar se os revisadores são necessários para fornecer justificativa com sua decisão.</span><span class="sxs-lookup"><span data-stu-id="62a78-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="62a78-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="62a78-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="62a78-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="62a78-120">Boolean</span></span> | <span data-ttu-id="62a78-121">Sinalizador para indicar se a decisão padrão está habilitada/desabilitada quando os revisadores não respondem.</span><span class="sxs-lookup"><span data-stu-id="62a78-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="62a78-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="62a78-122">defaultDecision</span></span>|<span data-ttu-id="62a78-123">String</span><span class="sxs-lookup"><span data-stu-id="62a78-123">String</span></span> | <span data-ttu-id="62a78-124">Decisão escolhida se `defaultDecisionEnabled` estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="62a78-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="62a78-125">Pode ser um de "Aprovar", "Negar" ou "Recomendação".</span><span class="sxs-lookup"><span data-stu-id="62a78-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="62a78-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="62a78-126">instanceDurationInDays</span></span>|<span data-ttu-id="62a78-127">Int32</span><span class="sxs-lookup"><span data-stu-id="62a78-127">Int32</span></span> | <span data-ttu-id="62a78-128">Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias.</span><span class="sxs-lookup"><span data-stu-id="62a78-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="62a78-129">recorrência</span><span class="sxs-lookup"><span data-stu-id="62a78-129">recurrence</span></span>|[<span data-ttu-id="62a78-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="62a78-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="62a78-131">Configurações detalhadas para recorrência.</span><span class="sxs-lookup"><span data-stu-id="62a78-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="62a78-132">Usando o objeto de recorrência padrão do Outlook.</span><span class="sxs-lookup"><span data-stu-id="62a78-132">Using standard Outlook recurrence object.</span></span> <span data-ttu-id="62a78-133">Observe que dayOfMonth não tem suporte - use a propriedade startDate em recurrenceRange para determinar o dia em que a revisão será iniciada.</span><span class="sxs-lookup"><span data-stu-id="62a78-133">Note that dayOfMonth is not supported - use property startDate on recurrenceRange to determine the day the review will start on.</span></span> |
| <span data-ttu-id="62a78-134">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="62a78-134">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="62a78-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="62a78-135">Boolean</span></span> | <span data-ttu-id="62a78-136">Sinalizador para indicar se o recurso de aplicação automática está habilitado.</span><span class="sxs-lookup"><span data-stu-id="62a78-136">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="62a78-137">applyActions</span><span class="sxs-lookup"><span data-stu-id="62a78-137">applyActions</span></span>|<span data-ttu-id="62a78-138">[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="62a78-138">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="62a78-139">Campo opcional.</span><span class="sxs-lookup"><span data-stu-id="62a78-139">Optional field.</span></span> <span data-ttu-id="62a78-140">Descreve as ações a ser realizadas depois que uma revisão é concluída.</span><span class="sxs-lookup"><span data-stu-id="62a78-140">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="62a78-141">Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="62a78-141">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="62a78-142">O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="62a78-142">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="62a78-143">Consulte [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="62a78-143">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="62a78-144">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="62a78-144">recommendationsEnabled</span></span>|<span data-ttu-id="62a78-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="62a78-145">Boolean</span></span> | <span data-ttu-id="62a78-146">Sinalizador para indicar se as recomendações de decisão estão habilitadas/desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="62a78-146">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="62a78-147">Relações</span><span class="sxs-lookup"><span data-stu-id="62a78-147">Relationships</span></span>
<span data-ttu-id="62a78-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62a78-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62a78-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62a78-149">JSON representation</span></span>
<span data-ttu-id="62a78-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62a78-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
