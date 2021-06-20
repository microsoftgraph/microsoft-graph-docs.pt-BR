---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize as propriedades de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 54b66ade8eb217ce740d3d721fc7433c9d86f505
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030993"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="6b194-103">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="6b194-103">Update accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="6b194-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b194-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b194-105">Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b194-105">Update the properties of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="6b194-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b194-106">Permissions</span></span>
<span data-ttu-id="6b194-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b194-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b194-109">Permission type</span></span>|<span data-ttu-id="6b194-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b194-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b194-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b194-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b194-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b194-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="6b194-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b194-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b194-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b194-114">Not supported.</span></span>|
|<span data-ttu-id="6b194-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b194-115">Application</span></span>|<span data-ttu-id="6b194-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b194-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="6b194-117">Somente um usuário de chamada listado como revisor do [accessReviewInstance](../resources/accessreviewinstance.md) pai pode atualizar **o accessReviewInstanceDecisionItem**.</span><span class="sxs-lookup"><span data-stu-id="6b194-117">Only a calling user who is listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md) can update the **accessReviewInstanceDecisionItem**.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b194-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b194-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="6b194-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b194-119">Request headers</span></span>
|<span data-ttu-id="6b194-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6b194-120">Name</span></span>|<span data-ttu-id="6b194-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b194-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6b194-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b194-122">Authorization</span></span>|<span data-ttu-id="6b194-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b194-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6b194-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b194-125">Content-Type</span></span>|<span data-ttu-id="6b194-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b194-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b194-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b194-128">Request body</span></span>
<span data-ttu-id="6b194-129">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="6b194-129">In the request body, supply a JSON representation of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

<span data-ttu-id="6b194-130">A tabela a seguir mostra as propriedades que são aceitas quando você atualiza [o accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="6b194-130">The following table shows the properties that are accepted when you update the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

|<span data-ttu-id="6b194-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b194-131">Property</span></span>|<span data-ttu-id="6b194-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b194-132">Type</span></span>|<span data-ttu-id="6b194-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b194-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b194-134">decision</span><span class="sxs-lookup"><span data-stu-id="6b194-134">decision</span></span>|<span data-ttu-id="6b194-135">String</span><span class="sxs-lookup"><span data-stu-id="6b194-135">String</span></span>|<span data-ttu-id="6b194-136">O voto do revistor sobre se a entidade deve ter acesso ao recurso em revisão.</span><span class="sxs-lookup"><span data-stu-id="6b194-136">The reviewer's vote on whether the principal should have access to the resource under review.</span></span> <span data-ttu-id="6b194-137">Valores possíveis: `Approve` `Deny` , ou `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="6b194-137">Possible values: `Approve`, `Deny`, or `DontKnow`.</span></span> <span data-ttu-id="6b194-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b194-138">Required.</span></span>|
|<span data-ttu-id="6b194-139">justification</span><span class="sxs-lookup"><span data-stu-id="6b194-139">justification</span></span>|<span data-ttu-id="6b194-140">String</span><span class="sxs-lookup"><span data-stu-id="6b194-140">String</span></span>|<span data-ttu-id="6b194-141">O motivo da decisão do revistor.</span><span class="sxs-lookup"><span data-stu-id="6b194-141">The reviewer's reason for decision.</span></span> <span data-ttu-id="6b194-142">Obrigatório se a **justificationRequiredOnApproval** da propriedade settings do [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) for `true` .</span><span class="sxs-lookup"><span data-stu-id="6b194-142">Required if the **justificationRequiredOnApproval** of the settings property of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="6b194-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b194-143">Response</span></span>

<span data-ttu-id="6b194-144">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="6b194-144">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6b194-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6b194-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b194-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b194-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json
Content-length: 691

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
}
```


### <a name="response"></a><span data-ttu-id="6b194-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b194-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
