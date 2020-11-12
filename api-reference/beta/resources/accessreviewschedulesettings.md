---
title: tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões do Azure AD Access, o `accessReviewScheduleSettings` representa as configurações associadas a uma série de análise do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cca1fa7fd0da05719c22728dd472087d9737d4e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000769"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="8aec4-103">tipo de recurso accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="8aec4-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="8aec4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aec4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aec4-105">O **accessReviewScheduleSettings** define as configurações de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8aec4-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="8aec4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8aec4-106">Properties</span></span>
| <span data-ttu-id="8aec4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aec4-107">Property</span></span>    | <span data-ttu-id="8aec4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aec4-108">Type</span></span>   | <span data-ttu-id="8aec4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aec4-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="8aec4-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="8aec4-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="8aec4-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec4-111">Boolean</span></span> | <span data-ttu-id="8aec4-112">Sinalizador para indicar se os emails estão habilitados/desabilitados.</span><span class="sxs-lookup"><span data-stu-id="8aec4-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="8aec4-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="8aec4-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="8aec4-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec4-114">Boolean</span></span>  | <span data-ttu-id="8aec4-115">Sinalizador para indicar se lembretes estão habilitados/desabilitados.</span><span class="sxs-lookup"><span data-stu-id="8aec4-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="8aec4-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="8aec4-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="8aec4-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec4-117">Boolean</span></span> | <span data-ttu-id="8aec4-118">Sinalizador para indicar se os revisores são necessários para fornecer justificação à sua decisão.</span><span class="sxs-lookup"><span data-stu-id="8aec4-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="8aec4-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="8aec4-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="8aec4-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec4-120">Boolean</span></span> | <span data-ttu-id="8aec4-121">Sinalizador para indicar se a decisão padrão será habilitada/desabilitada quando os revisores não responderem.</span><span class="sxs-lookup"><span data-stu-id="8aec4-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="8aec4-122">decisão</span><span class="sxs-lookup"><span data-stu-id="8aec4-122">defaultDecision</span></span>|<span data-ttu-id="8aec4-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aec4-123">String</span></span> | <span data-ttu-id="8aec4-124">Decisão escolhida se `defaultDecisionEnabled` estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="8aec4-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="8aec4-125">Pode ser uma das "aprovar", "negar" ou "recomendação".</span><span class="sxs-lookup"><span data-stu-id="8aec4-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="8aec4-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="8aec4-126">instanceDurationInDays</span></span>|<span data-ttu-id="8aec4-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8aec4-127">Int32</span></span> | <span data-ttu-id="8aec4-128">Duração de cada recorrência de Review ( `accessReviewInstance` ) em número de dias.</span><span class="sxs-lookup"><span data-stu-id="8aec4-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="8aec4-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="8aec4-129">recurrence</span></span>|[<span data-ttu-id="8aec4-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8aec4-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="8aec4-131">Definições detalhadas de recorrência.</span><span class="sxs-lookup"><span data-stu-id="8aec4-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="8aec4-132">Usando o objeto recorrência padrão do Outlook.</span><span class="sxs-lookup"><span data-stu-id="8aec4-132">Using standard Outlook recurrence object.</span></span>  |
| <span data-ttu-id="8aec4-133">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="8aec4-133">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="8aec4-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec4-134">Boolean</span></span> | <span data-ttu-id="8aec4-135">Sinalizador para indicar se o recurso de aplicação automática está habilitado.</span><span class="sxs-lookup"><span data-stu-id="8aec4-135">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="8aec4-136">applyActions</span><span class="sxs-lookup"><span data-stu-id="8aec4-136">applyActions</span></span>|<span data-ttu-id="8aec4-137">coleção [accessReviewApplyAction](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="8aec4-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="8aec4-138">Campo opcional.</span><span class="sxs-lookup"><span data-stu-id="8aec4-138">Optional field.</span></span> <span data-ttu-id="8aec4-139">Descreve as ações a serem tomadas após a conclusão da revisão.</span><span class="sxs-lookup"><span data-stu-id="8aec4-139">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="8aec4-140">Há dois tipos suportados atualmente: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="8aec4-140">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="8aec4-141">Field só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="8aec4-141">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="8aec4-142">Consulte [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="8aec4-142">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="8aec4-143">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="8aec4-143">recommendationsEnabled</span></span>|<span data-ttu-id="8aec4-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec4-144">Boolean</span></span> | <span data-ttu-id="8aec4-145">Sinalizador para indicar se as recomendações de decisão estão habilitadas/desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="8aec4-145">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8aec4-146">Relações</span><span class="sxs-lookup"><span data-stu-id="8aec4-146">Relationships</span></span>
<span data-ttu-id="8aec4-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8aec4-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8aec4-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8aec4-148">JSON representation</span></span>
<span data-ttu-id="8aec4-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8aec4-149">The following is a JSON representation of the resource.</span></span>
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
