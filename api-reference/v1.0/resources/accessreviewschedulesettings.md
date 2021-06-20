---
title: Tipo de recurso accessReviewScheduleSettings
description: Representa as configurações associadas a uma série de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8120d5b9b40f5e2ad744b65dcf927516e1d868b8
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030975"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="96555-103">Tipo de recurso accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="96555-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="96555-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96555-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96555-105">O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="96555-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="96555-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96555-106">Properties</span></span>
|<span data-ttu-id="96555-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96555-107">Property</span></span>|<span data-ttu-id="96555-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="96555-108">Type</span></span>|<span data-ttu-id="96555-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="96555-109">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="96555-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="96555-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="96555-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="96555-111">Boolean</span></span> | <span data-ttu-id="96555-112">Indica se os emails estão habilitados ou desabilitados.</span><span class="sxs-lookup"><span data-stu-id="96555-112">Indicates whether emails are enabled or disabled.</span></span> <span data-ttu-id="96555-113">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="96555-113">Default value is `false`.</span></span>               |
| <span data-ttu-id="96555-114">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="96555-114">reminderNotificationsEnabled</span></span>|<span data-ttu-id="96555-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="96555-115">Boolean</span></span>  | <span data-ttu-id="96555-116">Indica se os lembretes estão habilitados ou desabilitados.</span><span class="sxs-lookup"><span data-stu-id="96555-116">Indicates whether reminders are enabled or disabled.</span></span> <span data-ttu-id="96555-117">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="96555-117">Default value is `false`.</span></span>  |
| <span data-ttu-id="96555-118">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="96555-118">justificationRequiredOnApproval</span></span>|<span data-ttu-id="96555-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="96555-119">Boolean</span></span> | <span data-ttu-id="96555-120">Indica se os revisadores são necessários para fornecer justificativa com sua decisão.</span><span class="sxs-lookup"><span data-stu-id="96555-120">Indicates whether reviewers are required to provide justification with their decision.</span></span> <span data-ttu-id="96555-121">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="96555-121">Default value is `false`.</span></span> |
| <span data-ttu-id="96555-122">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="96555-122">defaultDecisionEnabled</span></span>|<span data-ttu-id="96555-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="96555-123">Boolean</span></span> | <span data-ttu-id="96555-124">Indica se a decisão padrão está habilitada ou desabilitada quando os revisadores não respondem.</span><span class="sxs-lookup"><span data-stu-id="96555-124">Indicates whether the default decision is enabled or disabled when reviewers do not respond.</span></span> <span data-ttu-id="96555-125">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="96555-125">Default value is `false`.</span></span> |
| <span data-ttu-id="96555-126">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="96555-126">defaultDecision</span></span>|<span data-ttu-id="96555-127">String</span><span class="sxs-lookup"><span data-stu-id="96555-127">String</span></span> | <span data-ttu-id="96555-128">Decisão escolhida se **defaultDecisionEnabled** for `true` .</span><span class="sxs-lookup"><span data-stu-id="96555-128">Decision chosen if **defaultDecisionEnabled** is `true`.</span></span> <span data-ttu-id="96555-129">Pode ser um `Approve` dos `Deny` , ou `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="96555-129">Can be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |
| <span data-ttu-id="96555-130">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="96555-130">instanceDurationInDays</span></span>|<span data-ttu-id="96555-131">Int32</span><span class="sxs-lookup"><span data-stu-id="96555-131">Int32</span></span> | <span data-ttu-id="96555-132">Duração de cada recorrência de revisão (**accessReviewInstance**) em número de dias.</span><span class="sxs-lookup"><span data-stu-id="96555-132">Duration of each recurrence of review (**accessReviewInstance**) in number of days.</span></span> |
| <span data-ttu-id="96555-133">recurrence</span><span class="sxs-lookup"><span data-stu-id="96555-133">recurrence</span></span>|[<span data-ttu-id="96555-134">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="96555-134">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="96555-135">Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão.</span><span class="sxs-lookup"><span data-stu-id="96555-135">Detailed settings for recurrence using the standard Outlook recurrence object.</span></span> <span data-ttu-id="96555-136">Somente `weekly` e `absoluteMonthly` em **recorrênciaPattern** são suportados.</span><span class="sxs-lookup"><span data-stu-id="96555-136">Only `weekly` and `absoluteMonthly` on **recurrencePattern** are supported.</span></span> <span data-ttu-id="96555-137">Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada.</span><span class="sxs-lookup"><span data-stu-id="96555-137">Use the property **startDate** on **recurrenceRange** to determine the day the review starts.</span></span> |
| <span data-ttu-id="96555-138">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="96555-138">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="96555-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="96555-139">Boolean</span></span> | <span data-ttu-id="96555-140">Indica se as decisões são aplicadas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="96555-140">Indicates whether decisions are automatically applied.</span></span> <span data-ttu-id="96555-141">Quando definido como , um usuário deve aplicar as decisões manualmente depois que o `false` revistor concluir a revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="96555-141">When set to `false`, a user must apply the decisions manually once the reviewer completes the access review.</span></span> <span data-ttu-id="96555-142">Quando definido como , as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os `true` revisadores responderam ou não.</span><span class="sxs-lookup"><span data-stu-id="96555-142">When set to `true`, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.</span></span> <span data-ttu-id="96555-143">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="96555-143">Default value is `false`.</span></span> |
| <span data-ttu-id="96555-144">applyActions</span><span class="sxs-lookup"><span data-stu-id="96555-144">applyActions</span></span>|<span data-ttu-id="96555-145">[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="96555-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="96555-146">Campo opcional.</span><span class="sxs-lookup"><span data-stu-id="96555-146">Optional field.</span></span> <span data-ttu-id="96555-147">Descreve as ações a ser realizadas depois que uma revisão é concluída.</span><span class="sxs-lookup"><span data-stu-id="96555-147">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="96555-148">Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="96555-148">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="96555-149">O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="96555-149">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="96555-150">Consulte [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="96555-150">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="96555-151">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="96555-151">recommendationsEnabled</span></span>|<span data-ttu-id="96555-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="96555-152">Boolean</span></span> | <span data-ttu-id="96555-153">Indica se as recomendações de decisão estão habilitadas ou desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="96555-153">Indicates whether decision recommendations are enabled or disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96555-154">Relações</span><span class="sxs-lookup"><span data-stu-id="96555-154">Relationships</span></span>
<span data-ttu-id="96555-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96555-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96555-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96555-156">JSON representation</span></span>
<span data-ttu-id="96555-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96555-157">The following is a JSON representation of the resource.</span></span>
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
