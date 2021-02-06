---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a `accessReviewScheduleSettings` uma série de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a58ba9a682e443efbc159befaea61b15e3fdc81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133440"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="6b55e-103">Tipo de recurso accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="6b55e-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="6b55e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b55e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b55e-105">**AccessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6b55e-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="6b55e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b55e-106">Properties</span></span>
| <span data-ttu-id="6b55e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b55e-107">Property</span></span>    | <span data-ttu-id="6b55e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b55e-108">Type</span></span>   | <span data-ttu-id="6b55e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b55e-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="6b55e-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6b55e-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="6b55e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b55e-111">Boolean</span></span> | <span data-ttu-id="6b55e-112">Sinalizador para indicar se os emails estão habilitados/desabilitados.</span><span class="sxs-lookup"><span data-stu-id="6b55e-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="6b55e-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6b55e-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="6b55e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b55e-114">Boolean</span></span>  | <span data-ttu-id="6b55e-115">Sinalizador para indicar se os lembretes estão habilitados/desabilitados.</span><span class="sxs-lookup"><span data-stu-id="6b55e-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="6b55e-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="6b55e-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="6b55e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b55e-117">Boolean</span></span> | <span data-ttu-id="6b55e-118">Sinalizador para indicar se os revisadores são obrigados a fornecer justificativa com sua decisão.</span><span class="sxs-lookup"><span data-stu-id="6b55e-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="6b55e-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="6b55e-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="6b55e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b55e-120">Boolean</span></span> | <span data-ttu-id="6b55e-121">Sinalizador para indicar se a decisão padrão está habilitada/desabilitada quando os revisadores não respondem.</span><span class="sxs-lookup"><span data-stu-id="6b55e-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="6b55e-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="6b55e-122">defaultDecision</span></span>|<span data-ttu-id="6b55e-123">String</span><span class="sxs-lookup"><span data-stu-id="6b55e-123">String</span></span> | <span data-ttu-id="6b55e-124">Decisão escolhida se `defaultDecisionEnabled` estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="6b55e-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="6b55e-125">Pode ser "Aprovar", "Negar" ou "Recomendação".</span><span class="sxs-lookup"><span data-stu-id="6b55e-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="6b55e-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="6b55e-126">instanceDurationInDays</span></span>|<span data-ttu-id="6b55e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6b55e-127">Int32</span></span> | <span data-ttu-id="6b55e-128">Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias.</span><span class="sxs-lookup"><span data-stu-id="6b55e-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="6b55e-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="6b55e-129">recurrence</span></span>|[<span data-ttu-id="6b55e-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6b55e-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="6b55e-131">Configurações detalhadas de recorrência.</span><span class="sxs-lookup"><span data-stu-id="6b55e-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="6b55e-132">Usando o objeto de recorrência padrão do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6b55e-132">Using standard Outlook recurrence object.</span></span>  |
| <span data-ttu-id="6b55e-133">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="6b55e-133">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="6b55e-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b55e-134">Boolean</span></span> | <span data-ttu-id="6b55e-135">Sinalizador para indicar se o recurso de aplicação automática está habilitado.</span><span class="sxs-lookup"><span data-stu-id="6b55e-135">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="6b55e-136">applyActions</span><span class="sxs-lookup"><span data-stu-id="6b55e-136">applyActions</span></span>|<span data-ttu-id="6b55e-137">[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="6b55e-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="6b55e-138">Campo opcional.</span><span class="sxs-lookup"><span data-stu-id="6b55e-138">Optional field.</span></span> <span data-ttu-id="6b55e-139">Descreve as ações a tomar depois que uma revisão é concluída.</span><span class="sxs-lookup"><span data-stu-id="6b55e-139">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="6b55e-140">Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="6b55e-140">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="6b55e-141">O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="6b55e-141">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="6b55e-142">Consulte [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="6b55e-142">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="6b55e-143">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6b55e-143">recommendationsEnabled</span></span>|<span data-ttu-id="6b55e-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b55e-144">Boolean</span></span> | <span data-ttu-id="6b55e-145">Sinalizador para indicar se as recomendações de decisão estão habilitadas/desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="6b55e-145">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6b55e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="6b55e-146">Relationships</span></span>
<span data-ttu-id="6b55e-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b55e-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b55e-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b55e-148">JSON representation</span></span>
<span data-ttu-id="6b55e-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b55e-149">The following is a JSON representation of the resource.</span></span>
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
