---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a0003ab8a79372a4dfefea1a62120ea8e40fa2c1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443192"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="b7899-103">Tipo de recurso accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b7899-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="b7899-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7899-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="b7899-105">Representa uma recorrência de revisão de acesso [do](accessreviewsv2-root.md) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7899-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="b7899-106">Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai for uma revisão de acesso recorrente, as instâncias representarão cada recorrência.</span><span class="sxs-lookup"><span data-stu-id="b7899-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="b7899-107">Uma revisão que não se recorre terá exatamente uma instância.</span><span class="sxs-lookup"><span data-stu-id="b7899-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="b7899-108">As instâncias também representam cada grupo exclusivo que está sendo revisado na definição de agendamento.</span><span class="sxs-lookup"><span data-stu-id="b7899-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="b7899-109">Se uma definição de agenda analisar vários grupos, cada grupo terá uma instância exclusiva para cada recorrência.</span><span class="sxs-lookup"><span data-stu-id="b7899-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="b7899-110">Cada **accessReviewInstance** contém uma lista de [decisões](accessreviewinstancedecisionitem.md) que os revisores podem tomar medidas.</span><span class="sxs-lookup"><span data-stu-id="b7899-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="b7899-111">Há uma decisão por identidade sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="b7899-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="b7899-112">Methods</span><span class="sxs-lookup"><span data-stu-id="b7899-112">Methods</span></span>

| <span data-ttu-id="b7899-113">Método</span><span class="sxs-lookup"><span data-stu-id="b7899-113">Method</span></span> | <span data-ttu-id="b7899-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b7899-114">Return Type</span></span> | <span data-ttu-id="b7899-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7899-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7899-116">Listar accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="b7899-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="b7899-117">[Coleção accessReviewInstance](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="b7899-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="b7899-118">Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b7899-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="b7899-119">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b7899-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="b7899-120">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b7899-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="b7899-121">Retorna accessReviewInstance para um accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="b7899-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="b7899-122">Não inclui accessReviewInstanceDecisionItem associado no objeto.</span><span class="sxs-lookup"><span data-stu-id="b7899-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="b7899-123">Listar pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="b7899-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="b7899-124">[Coleção accessReviewInstance.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="b7899-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="b7899-125">Obter todos os recursos de accessReviewInstance pendentes atribuídos ao usuário de chamada.</span><span class="sxs-lookup"><span data-stu-id="b7899-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="b7899-126">Enviar lembrete accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b7899-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="b7899-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7899-127">None.</span></span> | <span data-ttu-id="b7899-128">Envie um lembrete aos revisores de um accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="b7899-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="b7899-129">Parar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b7899-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="b7899-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7899-130">None.</span></span> | <span data-ttu-id="b7899-131">Pare manualmente um accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="b7899-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="b7899-132">Aceitar recomendações</span><span class="sxs-lookup"><span data-stu-id="b7899-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="b7899-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7899-133">None.</span></span> | <span data-ttu-id="b7899-134">Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="b7899-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="b7899-135">Aplicar decisões</span><span class="sxs-lookup"><span data-stu-id="b7899-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="b7899-136">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7899-136">None.</span></span> | <span data-ttu-id="b7899-137">Aplicar manualmente a decisão em um accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="b7899-137">Manually apply decision on an accessReviewInstance.</span></span> |



## <a name="properties"></a><span data-ttu-id="b7899-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7899-138">Properties</span></span>
| <span data-ttu-id="b7899-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7899-139">Property</span></span> | <span data-ttu-id="b7899-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7899-140">Type</span></span> | <span data-ttu-id="b7899-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7899-141">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="b7899-142">id</span><span class="sxs-lookup"><span data-stu-id="b7899-142">id</span></span> | <span data-ttu-id="b7899-143">String</span><span class="sxs-lookup"><span data-stu-id="b7899-143">String</span></span> | <span data-ttu-id="b7899-144">Identificador exclusivo da instância.</span><span class="sxs-lookup"><span data-stu-id="b7899-144">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="b7899-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b7899-145">displayName</span></span> | <span data-ttu-id="b7899-146">String</span><span class="sxs-lookup"><span data-stu-id="b7899-146">String</span></span> | <span data-ttu-id="b7899-147">Nome do access paiReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="b7899-147">Name of the parent accessReviewScheduleDefinition.</span></span> |
| <span data-ttu-id="b7899-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b7899-148">startDateTime</span></span> | <span data-ttu-id="b7899-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7899-149">DateTimeOffset</span></span> | <span data-ttu-id="b7899-150">DateTime quando a instância de revisão está agendada para começar.</span><span class="sxs-lookup"><span data-stu-id="b7899-150">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="b7899-151">Pode ser no futuro.</span><span class="sxs-lookup"><span data-stu-id="b7899-151">May be in the future.</span></span> |
| <span data-ttu-id="b7899-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b7899-152">endDateTime</span></span> | <span data-ttu-id="b7899-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7899-153">DateTimeOffset</span></span> | <span data-ttu-id="b7899-154">DateTime quando a instância de revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="b7899-154">DateTime when review instance is scheduled to end.</span></span> |
| <span data-ttu-id="b7899-155">status</span><span class="sxs-lookup"><span data-stu-id="b7899-155">status</span></span> | <span data-ttu-id="b7899-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7899-156">string</span></span> | <span data-ttu-id="b7899-157">Especifica o status de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="b7899-157">Specifies the status of an accessReview.</span></span> <span data-ttu-id="b7899-158">Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .</span><span class="sxs-lookup"><span data-stu-id="b7899-158">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="b7899-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7899-159">Read-only.</span></span>|
| <span data-ttu-id="b7899-160">escopo</span><span class="sxs-lookup"><span data-stu-id="b7899-160">scope</span></span> | [<span data-ttu-id="b7899-161">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="b7899-161">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="b7899-162">Criado com base **no escopo** e **instanceEnumerationScope** no nível accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="b7899-162">Created based on **scope** and **instanceEnumerationScope** at the accessReviewScheduleDefinition level.</span></span> <span data-ttu-id="b7899-163">Define o escopo dos usuários revisados em um grupo.</span><span class="sxs-lookup"><span data-stu-id="b7899-163">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="b7899-164">No caso de uma revisão de grupo único, o escopo definido no `accessReviewScheduleDefinition` nível se aplica a todas as instâncias.</span><span class="sxs-lookup"><span data-stu-id="b7899-164">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="b7899-165">No caso da revisão de todos os grupos, o escopo pode ser diferente para cada grupo.</span><span class="sxs-lookup"><span data-stu-id="b7899-165">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="b7899-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b7899-166">Read-only.</span></span>  | 
| <span data-ttu-id="b7899-167">decisions</span><span class="sxs-lookup"><span data-stu-id="b7899-167">decisions</span></span> | <span data-ttu-id="b7899-168">[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="b7899-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="b7899-169">Cada usuário revisado em um accessReviewInstance tem um item de decisão que representa se seu acesso foi aprovado, negado ou ainda não revisado.</span><span class="sxs-lookup"><span data-stu-id="b7899-169">Each user reviewed in an accessReviewInstance has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="b7899-170">definition</span><span class="sxs-lookup"><span data-stu-id="b7899-170">definition</span></span> |[<span data-ttu-id="b7899-171">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="b7899-171">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="b7899-172">Há exatamente um accessReviewScheduleDefinition associado a cada instância.</span><span class="sxs-lookup"><span data-stu-id="b7899-172">There is exactly one accessReviewScheduleDefinition associated with each instance.</span></span> <span data-ttu-id="b7899-173">É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição.</span><span class="sxs-lookup"><span data-stu-id="b7899-173">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b7899-174">Relações</span><span class="sxs-lookup"><span data-stu-id="b7899-174">Relationships</span></span>

| <span data-ttu-id="b7899-175">Relação</span><span class="sxs-lookup"><span data-stu-id="b7899-175">Relationship</span></span> | <span data-ttu-id="b7899-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7899-176">Type</span></span>   |<span data-ttu-id="b7899-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7899-177">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="b7899-178">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="b7899-178">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="b7899-179">Há exatamente um `accessReviewScheduleDefinition` associado a cada instância.</span><span class="sxs-lookup"><span data-stu-id="b7899-179">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="b7899-180">É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição.</span><span class="sxs-lookup"><span data-stu-id="b7899-180">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="b7899-181">[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="b7899-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="b7899-182">Cada usuário revisado em um tem um item de decisão representando se eles foram `accessReviewInstance` aprovados, negados ou ainda não revisados.</span><span class="sxs-lookup"><span data-stu-id="b7899-182">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b7899-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7899-183">JSON representation</span></span>

<span data-ttu-id="b7899-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7899-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
