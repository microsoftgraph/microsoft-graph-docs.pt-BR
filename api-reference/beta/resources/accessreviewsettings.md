---
title: tipo de recurso accessReviewSettings
description: Fornece configurações adicionais ao criar uma revisão do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4de925ecb2fac65e3ab339ba8d4e602fcdc2af3
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330351"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="410d2-103">tipo de recurso accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="410d2-103">accessReviewSettings resource type</span></span>

<span data-ttu-id="410d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="410d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="410d2-105">Fornece configurações adicionais ao criar uma revisão do Access, para controlar o comportamento do recurso ao iniciar uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="410d2-105">Provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>

## <a name="properties"></a><span data-ttu-id="410d2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="410d2-106">Properties</span></span>

| <span data-ttu-id="410d2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="410d2-107">Property</span></span> | <span data-ttu-id="410d2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="410d2-108">Type</span></span> | <span data-ttu-id="410d2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="410d2-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="410d2-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="410d2-110">mailNotificationsEnabled</span></span> | <span data-ttu-id="410d2-111">Booleano</span><span class="sxs-lookup"><span data-stu-id="410d2-111">Boolean</span></span> | <span data-ttu-id="410d2-112">Indica se o envio de emails para revisores e o criador de revisão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="410d2-112">Indicates whether sending mails to reviewers and the review creator is enabled.</span></span> |
| <span data-ttu-id="410d2-113">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="410d2-113">remindersEnabled</span></span> | <span data-ttu-id="410d2-114">Booleano</span><span class="sxs-lookup"><span data-stu-id="410d2-114">Boolean</span></span> | <span data-ttu-id="410d2-115">Indica se o envio de emails de lembrete aos revisores está habilitado.</span><span class="sxs-lookup"><span data-stu-id="410d2-115">Indicates whether sending reminder emails to reviewers is enabled.</span></span> |
| <span data-ttu-id="410d2-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="410d2-116">justificationRequiredOnApproval</span></span> | <span data-ttu-id="410d2-117">Booleano</span><span class="sxs-lookup"><span data-stu-id="410d2-117">Boolean</span></span> | <span data-ttu-id="410d2-118">Indica se os revisores são necessários para fornecer uma justificativa ao revisar o acesso.</span><span class="sxs-lookup"><span data-stu-id="410d2-118">Indicates whether reviewers are required to provide a justification when reviewing access.</span></span> |
| <span data-ttu-id="410d2-119">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="410d2-119">activityDurationInDays</span></span> | <span data-ttu-id="410d2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="410d2-120">Int64</span></span> | <span data-ttu-id="410d2-121">O número de dias de atividades do usuário para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="410d2-121">The number of days of user activities to show to reviewers.</span></span> |
| <span data-ttu-id="410d2-122">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="410d2-122">autoReviewEnabled</span></span> | <span data-ttu-id="410d2-123">Booleano</span><span class="sxs-lookup"><span data-stu-id="410d2-123">Boolean</span></span> | <span data-ttu-id="410d2-124">Indica se uma decisão deverá ser definida se o revisor não fornecer um.</span><span class="sxs-lookup"><span data-stu-id="410d2-124">Indicates whether a decision should be set if the reviewer did not supply one.</span></span> <span data-ttu-id="410d2-125">Para uso quando a aplicação automática está habilitada.</span><span class="sxs-lookup"><span data-stu-id="410d2-125">For use when auto-apply is enabled.</span></span> <span data-ttu-id="410d2-126">Se você não quiser ter uma decisão de revisão registrada, a menos que o revisor faça uma escolha explícita, defina-a como `false` .</span><span class="sxs-lookup"><span data-stu-id="410d2-126">If you don't want to have a review decision recorded unless the reviewer makes an explicit choice, set it to `false`.</span></span>|
| <span data-ttu-id="410d2-127">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="410d2-127">autoReviewSettings</span></span> | [<span data-ttu-id="410d2-128">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="410d2-128">autoReviewSettings</span></span>](autoreviewsettings.md) | <span data-ttu-id="410d2-129">Configurações detalhadas de como o recurso deve definir a decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="410d2-129">Detailed settings for how the feature should set the review decision.</span></span> <span data-ttu-id="410d2-130">Para uso quando a aplicação automática está habilitada.</span><span class="sxs-lookup"><span data-stu-id="410d2-130">For use when auto-apply is enabled.</span></span> |
| <span data-ttu-id="410d2-131">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="410d2-131">recurrenceSettings</span></span> | [<span data-ttu-id="410d2-132">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="410d2-132">accessReviewRecurrenceSettings</span></span>](accessreviewrecurrencesettings.md) | <span data-ttu-id="410d2-133">Definições detalhadas de recorrência.</span><span class="sxs-lookup"><span data-stu-id="410d2-133">Detailed settings for recurrence.</span></span> |
| <span data-ttu-id="410d2-134">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="410d2-134">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="410d2-135">Booleano</span><span class="sxs-lookup"><span data-stu-id="410d2-135">Boolean</span></span> | <span data-ttu-id="410d2-136">Indica se o recurso de aplicação automática, para alterar automaticamente o recurso de acesso ao objeto de destino, está habilitado.</span><span class="sxs-lookup"><span data-stu-id="410d2-136">Indicates whether the auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="410d2-137">Se não habilitado, um usuário deve, após a conclusão da revisão, aplicar a revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="410d2-137">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| <span data-ttu-id="410d2-138">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="410d2-138">accessRecommendationsEnabled</span></span> | <span data-ttu-id="410d2-139">Booleano</span><span class="sxs-lookup"><span data-stu-id="410d2-139">Boolean</span></span> | <span data-ttu-id="410d2-140">Indica se a exibição de recomendações para revisores está habilitada.</span><span class="sxs-lookup"><span data-stu-id="410d2-140">Indicates whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="410d2-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="410d2-141">JSON representation</span></span>
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