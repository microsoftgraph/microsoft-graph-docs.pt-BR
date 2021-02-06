---
title: Tipo de recurso accessReviewSettings
description: Fornece configurações adicionais ao criar uma revisão de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18af2ef86c33650129934f43d2212222e98448fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133424"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="a960f-103">Tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="a960f-103">accessReviewSettings resource type</span></span>

<span data-ttu-id="a960f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a960f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a960f-105">Fornece configurações adicionais ao criar uma revisão de acesso, para controlar o comportamento do recurso ao iniciar uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a960f-105">Provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>

## <a name="properties"></a><span data-ttu-id="a960f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a960f-106">Properties</span></span>

| <span data-ttu-id="a960f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a960f-107">Property</span></span> | <span data-ttu-id="a960f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a960f-108">Type</span></span> | <span data-ttu-id="a960f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a960f-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="a960f-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="a960f-110">mailNotificationsEnabled</span></span> | <span data-ttu-id="a960f-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="a960f-111">Boolean</span></span> | <span data-ttu-id="a960f-112">Indica se o envio de emails aos revisadores e ao criador da crítica está habilitado.</span><span class="sxs-lookup"><span data-stu-id="a960f-112">Indicates whether sending mails to reviewers and the review creator is enabled.</span></span> |
| <span data-ttu-id="a960f-113">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="a960f-113">remindersEnabled</span></span> | <span data-ttu-id="a960f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a960f-114">Boolean</span></span> | <span data-ttu-id="a960f-115">Indica se o envio de emails de lembrete para revisadores está habilitado.</span><span class="sxs-lookup"><span data-stu-id="a960f-115">Indicates whether sending reminder emails to reviewers is enabled.</span></span> |
| <span data-ttu-id="a960f-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="a960f-116">justificationRequiredOnApproval</span></span> | <span data-ttu-id="a960f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a960f-117">Boolean</span></span> | <span data-ttu-id="a960f-118">Indica se os revisadores devem fornecer uma justificativa ao revisar o acesso.</span><span class="sxs-lookup"><span data-stu-id="a960f-118">Indicates whether reviewers are required to provide a justification when reviewing access.</span></span> |
| <span data-ttu-id="a960f-119">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="a960f-119">activityDurationInDays</span></span> | <span data-ttu-id="a960f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a960f-120">Int64</span></span> | <span data-ttu-id="a960f-121">O número de dias de atividades do usuário para mostrar aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="a960f-121">The number of days of user activities to show to reviewers.</span></span> |
| <span data-ttu-id="a960f-122">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="a960f-122">autoReviewEnabled</span></span> | <span data-ttu-id="a960f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a960f-123">Boolean</span></span> | <span data-ttu-id="a960f-124">Indica se uma decisão deve ser definida se o revistor não forneceu uma.</span><span class="sxs-lookup"><span data-stu-id="a960f-124">Indicates whether a decision should be set if the reviewer did not supply one.</span></span> <span data-ttu-id="a960f-125">Para uso quando a aplicação automática estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="a960f-125">For use when auto-apply is enabled.</span></span> <span data-ttu-id="a960f-126">Se você não quiser ter uma decisão de revisão registrada, a menos que o revistor faça uma escolha explícita, de definida como `false` .</span><span class="sxs-lookup"><span data-stu-id="a960f-126">If you don't want to have a review decision recorded unless the reviewer makes an explicit choice, set it to `false`.</span></span>|
| <span data-ttu-id="a960f-127">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="a960f-127">autoReviewSettings</span></span> | [<span data-ttu-id="a960f-128">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="a960f-128">autoReviewSettings</span></span>](autoreviewsettings.md) | <span data-ttu-id="a960f-129">Configurações detalhadas de como o recurso deve definir a decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="a960f-129">Detailed settings for how the feature should set the review decision.</span></span> <span data-ttu-id="a960f-130">Para uso quando a aplicação automática estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="a960f-130">For use when auto-apply is enabled.</span></span> |
| <span data-ttu-id="a960f-131">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="a960f-131">recurrenceSettings</span></span> | [<span data-ttu-id="a960f-132">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="a960f-132">accessReviewRecurrenceSettings</span></span>](accessreviewrecurrencesettings.md) | <span data-ttu-id="a960f-133">Configurações detalhadas de recorrência.</span><span class="sxs-lookup"><span data-stu-id="a960f-133">Detailed settings for recurrence.</span></span> |
| <span data-ttu-id="a960f-134">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="a960f-134">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="a960f-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a960f-135">Boolean</span></span> | <span data-ttu-id="a960f-136">Indica se a funcionalidade de aplicação automática, para alterar automaticamente o recurso de acesso ao objeto de destino, está habilitada.</span><span class="sxs-lookup"><span data-stu-id="a960f-136">Indicates whether the auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="a960f-137">Se não estiver habilitado, um usuário deverá, após a conclusão da revisão, aplicar a revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a960f-137">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| <span data-ttu-id="a960f-138">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="a960f-138">accessRecommendationsEnabled</span></span> | <span data-ttu-id="a960f-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="a960f-139">Boolean</span></span> | <span data-ttu-id="a960f-140">Indica se a exibição de recomendações para revisadores está habilitada.</span><span class="sxs-lookup"><span data-stu-id="a960f-140">Indicates whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a960f-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a960f-141">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
```json
{
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,  
  "justificationRequiredOnApproval": true,
  "activityDurationInDays": 1024,
  "autoReviewEnabled": false,
  "autoReviewSettings": {"@odata.type": "microsoft.graph.autoReviewSettings"},
  "recurrenceSettings": {"@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"},
  "autoApplyReviewResultsEnabled": false,
  "accessRecommendationsEnabled": false
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
