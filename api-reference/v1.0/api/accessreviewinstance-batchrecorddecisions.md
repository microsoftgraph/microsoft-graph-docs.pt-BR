---
title: 'accessReviewInstance: batchRecordDecisions'
description: Permite que os revisores revisem todos os accessReviewInstanceDecisionItems em lotes.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ea22d510bb70ab8d7047f952f7b4c0e265d57197
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031011"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="6ee89-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="6ee89-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="6ee89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ee89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ee89-105">Permite que os revisores revisem todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em lotes usando **principalId,** **resourceId** ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="6ee89-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ee89-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ee89-106">Permissions</span></span>
<span data-ttu-id="6ee89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ee89-109">Permission type</span></span>|<span data-ttu-id="6ee89-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ee89-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ee89-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ee89-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ee89-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee89-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="6ee89-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ee89-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ee89-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6ee89-114">Not supported</span></span>|
|<span data-ttu-id="6ee89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ee89-115">Application</span></span>|<span data-ttu-id="6ee89-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee89-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ee89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ee89-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="6ee89-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee89-118">Request headers</span></span>
|<span data-ttu-id="6ee89-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6ee89-119">Name</span></span>|<span data-ttu-id="6ee89-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ee89-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6ee89-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ee89-121">Authorization</span></span>|<span data-ttu-id="6ee89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ee89-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6ee89-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ee89-124">Content-Type</span></span>|<span data-ttu-id="6ee89-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ee89-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ee89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee89-127">Request body</span></span>
<span data-ttu-id="6ee89-128">No corpo da solicitação, fornece uma representação JSON de [um accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="6ee89-128">In the request body, supply a JSON representation of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="6ee89-129">A tabela a seguir lista as propriedades que você pode usar para revisar [objetos accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="6ee89-129">The following table lists the properties that you can use to review [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

|<span data-ttu-id="6ee89-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6ee89-130">Parameter</span></span>|<span data-ttu-id="6ee89-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ee89-131">Type</span></span>|<span data-ttu-id="6ee89-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ee89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ee89-133">decision</span><span class="sxs-lookup"><span data-stu-id="6ee89-133">decision</span></span>|<span data-ttu-id="6ee89-134">String</span><span class="sxs-lookup"><span data-stu-id="6ee89-134">String</span></span>|<span data-ttu-id="6ee89-135">Decisão de acesso para a entidade que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="6ee89-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="6ee89-136">Os valores possíveis são: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="6ee89-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="6ee89-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ee89-137">Required.</span></span>|
|<span data-ttu-id="6ee89-138">justification</span><span class="sxs-lookup"><span data-stu-id="6ee89-138">justification</span></span>|<span data-ttu-id="6ee89-139">String</span><span class="sxs-lookup"><span data-stu-id="6ee89-139">String</span></span>|<span data-ttu-id="6ee89-140">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="6ee89-140">Context of the review provided to admins.</span></span> <span data-ttu-id="6ee89-141">Obrigatório se **justificationRequiredOnApproval** da propriedade settings do **accessReviewScheduleDefinition** for `true` .</span><span class="sxs-lookup"><span data-stu-id="6ee89-141">Required if **justificationRequiredOnApproval** of the settings property of the **accessReviewScheduleDefinition** is `true` .</span></span>|
|<span data-ttu-id="6ee89-142">principalId</span><span class="sxs-lookup"><span data-stu-id="6ee89-142">principalId</span></span>|<span data-ttu-id="6ee89-143">String</span><span class="sxs-lookup"><span data-stu-id="6ee89-143">String</span></span>|<span data-ttu-id="6ee89-144">Se fornecido, todos os **accessReviewInstanceDecisionItems** com valores **principalId** correspondentes serão revisados neste lote.</span><span class="sxs-lookup"><span data-stu-id="6ee89-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** values will be reviewed in this batch.</span></span> <span data-ttu-id="6ee89-145">Se não for fornecido, **todos os accessReviewInstanceDecisionItems** serão revisados.</span><span class="sxs-lookup"><span data-stu-id="6ee89-145">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|
|<span data-ttu-id="6ee89-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="6ee89-146">resourceId</span></span>|<span data-ttu-id="6ee89-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ee89-147">String</span></span>|<span data-ttu-id="6ee89-148">Se fornecido, todos os **accessReviewInstanceDecisionItems** com **resourceId** correspondentes serão revisados neste lote.</span><span class="sxs-lookup"><span data-stu-id="6ee89-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="6ee89-149">Se não for fornecido, **todos os accessReviewInstanceDecisionItems** serão revisados.</span><span class="sxs-lookup"><span data-stu-id="6ee89-149">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|

## <a name="response"></a><span data-ttu-id="6ee89-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee89-150">Response</span></span>

<span data-ttu-id="6ee89-151">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6ee89-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6ee89-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6ee89-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ee89-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee89-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions
Content-type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```

### <a name="response"></a><span data-ttu-id="6ee89-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee89-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
