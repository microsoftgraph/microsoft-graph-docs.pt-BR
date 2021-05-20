---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a uma série de revisão `accessReviewScheduleSettings` de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b354ebfc2b5e6c8093f65c8712516421f0b1d332
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579729"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="88ea4-103">Tipo de recurso accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="88ea4-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="88ea4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ea4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="88ea4-105">O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="88ea4-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="88ea4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88ea4-106">Properties</span></span>
| <span data-ttu-id="88ea4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88ea4-107">Property</span></span>    | <span data-ttu-id="88ea4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="88ea4-108">Type</span></span>   | <span data-ttu-id="88ea4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="88ea4-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="88ea4-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="88ea4-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="88ea4-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ea4-111">Boolean</span></span> | <span data-ttu-id="88ea4-112">Indica se os emails estão habilitados ou desabilitados.</span><span class="sxs-lookup"><span data-stu-id="88ea4-112">Indicates whether emails are enabled or disabled.</span></span> <span data-ttu-id="88ea4-113">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="88ea4-113">Default value is `false`.</span></span>               |
| <span data-ttu-id="88ea4-114">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="88ea4-114">reminderNotificationsEnabled</span></span>|<span data-ttu-id="88ea4-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ea4-115">Boolean</span></span>  | <span data-ttu-id="88ea4-116">Indica se os lembretes estão habilitados ou desabilitados.</span><span class="sxs-lookup"><span data-stu-id="88ea4-116">Indicates whether reminders are enabled or disabled.</span></span> <span data-ttu-id="88ea4-117">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="88ea4-117">Default value is `false`.</span></span>  |
| <span data-ttu-id="88ea4-118">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="88ea4-118">justificationRequiredOnApproval</span></span>|<span data-ttu-id="88ea4-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ea4-119">Boolean</span></span> | <span data-ttu-id="88ea4-120">Indica se os revisadores são necessários para fornecer justificativa com sua decisão.</span><span class="sxs-lookup"><span data-stu-id="88ea4-120">Indicates whether reviewers are required to provide justification with their decision.</span></span> <span data-ttu-id="88ea4-121">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="88ea4-121">Default value is `false`.</span></span> |
| <span data-ttu-id="88ea4-122">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="88ea4-122">defaultDecisionEnabled</span></span>|<span data-ttu-id="88ea4-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ea4-123">Boolean</span></span> | <span data-ttu-id="88ea4-124">Indica se a decisão padrão está habilitada ou desabilitada quando os revisadores não respondem.</span><span class="sxs-lookup"><span data-stu-id="88ea4-124">Indicates whether the default decision is enabled or disabled when reviewers do not respond.</span></span> <span data-ttu-id="88ea4-125">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="88ea4-125">Default value is `false`.</span></span> |
| <span data-ttu-id="88ea4-126">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="88ea4-126">defaultDecision</span></span>|<span data-ttu-id="88ea4-127">String</span><span class="sxs-lookup"><span data-stu-id="88ea4-127">String</span></span> | <span data-ttu-id="88ea4-128">Decisão escolhida se `defaultDecisionEnabled` estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="88ea4-128">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="88ea4-129">Pode ser um `Approve` dos `Deny` , ou `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="88ea4-129">Can be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |
| <span data-ttu-id="88ea4-130">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="88ea4-130">instanceDurationInDays</span></span>|<span data-ttu-id="88ea4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea4-131">Int32</span></span> | <span data-ttu-id="88ea4-132">Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias.</span><span class="sxs-lookup"><span data-stu-id="88ea4-132">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="88ea4-133">recurrence</span><span class="sxs-lookup"><span data-stu-id="88ea4-133">recurrence</span></span>|[<span data-ttu-id="88ea4-134">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="88ea4-134">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="88ea4-135">Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão.</span><span class="sxs-lookup"><span data-stu-id="88ea4-135">Detailed settings for recurrence using the standard Outlook recurrence object.</span></span> <span data-ttu-id="88ea4-136">Somente `weekly` e `absoluteMonthly` em **recorrênciaPattern** são suportados.</span><span class="sxs-lookup"><span data-stu-id="88ea4-136">Only `weekly` and `absoluteMonthly` on **recurrencePattern** are supported.</span></span> <span data-ttu-id="88ea4-137">Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada.</span><span class="sxs-lookup"><span data-stu-id="88ea4-137">Use the property **startDate** on **recurrenceRange** to determine the day the review starts.</span></span> |
| <span data-ttu-id="88ea4-138">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="88ea4-138">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="88ea4-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ea4-139">Boolean</span></span> | <span data-ttu-id="88ea4-140">Indica se as decisões são aplicadas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="88ea4-140">Indicates whether decisions are automatically applied.</span></span> <span data-ttu-id="88ea4-141">Quando definido como , um usuário deve aplicar as decisões manualmente depois que o `false` revistor concluir a revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="88ea4-141">When set to `false`, a user must apply the decisions manually once the reviewer completes the access review.</span></span> <span data-ttu-id="88ea4-142">Quando definido como , as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os `true` revisadores responderam ou não.</span><span class="sxs-lookup"><span data-stu-id="88ea4-142">When set to `true`, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.</span></span> <span data-ttu-id="88ea4-143">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="88ea4-143">Default value is `false`.</span></span> |
| <span data-ttu-id="88ea4-144">applyActions</span><span class="sxs-lookup"><span data-stu-id="88ea4-144">applyActions</span></span>|<span data-ttu-id="88ea4-145">[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="88ea4-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="88ea4-146">Campo opcional.</span><span class="sxs-lookup"><span data-stu-id="88ea4-146">Optional field.</span></span> <span data-ttu-id="88ea4-147">Descreve as ações a ser realizadas depois que uma revisão é concluída.</span><span class="sxs-lookup"><span data-stu-id="88ea4-147">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="88ea4-148">Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="88ea4-148">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="88ea4-149">O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="88ea4-149">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="88ea4-150">Consulte [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="88ea4-150">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="88ea4-151">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="88ea4-151">recommendationsEnabled</span></span>|<span data-ttu-id="88ea4-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="88ea4-152">Boolean</span></span> | <span data-ttu-id="88ea4-153">Indica se as recomendações de decisão estão habilitadas/desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="88ea4-153">Indicates whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="88ea4-154">Relações</span><span class="sxs-lookup"><span data-stu-id="88ea4-154">Relationships</span></span>
<span data-ttu-id="88ea4-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88ea4-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="88ea4-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88ea4-156">JSON representation</span></span>
<span data-ttu-id="88ea4-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88ea4-157">The following is a JSON representation of the resource.</span></span>
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
