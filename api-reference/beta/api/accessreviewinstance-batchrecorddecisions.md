---
title: 'accessReviewInstance: batchRecordDecisions'
description: Revisores emable para revisar todos os accessReviewInstanceDecisionItems em lotes.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a8bd6778d54100340b0c846230fd8b91b696f1fb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507454"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="77c2a-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="77c2a-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="77c2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77c2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c2a-105">Permitir que os revisores revisem todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em lotes usando `principalId` , ou nenhum `resourceId` deles.</span><span class="sxs-lookup"><span data-stu-id="77c2a-105">Enable reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using `principalId`, `resourceId`, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="77c2a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="77c2a-106">Permissions</span></span>
<span data-ttu-id="77c2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77c2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77c2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77c2a-109">Permission type</span></span>|<span data-ttu-id="77c2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77c2a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77c2a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77c2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77c2a-112">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c2a-112">AccessReviews.ReadWrite.All</span></span>|
|<span data-ttu-id="77c2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77c2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77c2a-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="77c2a-114">Not supported</span></span>|
|<span data-ttu-id="77c2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77c2a-115">Application</span></span>|<span data-ttu-id="77c2a-116">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c2a-116">AccessReviews.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77c2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77c2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="77c2a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77c2a-118">Request headers</span></span>
|<span data-ttu-id="77c2a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="77c2a-119">Name</span></span>|<span data-ttu-id="77c2a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="77c2a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="77c2a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77c2a-121">Authorization</span></span>|<span data-ttu-id="77c2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77c2a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="77c2a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77c2a-124">Content-Type</span></span>|<span data-ttu-id="77c2a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77c2a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77c2a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77c2a-127">Request body</span></span>
<span data-ttu-id="77c2a-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="77c2a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="77c2a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="77c2a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="77c2a-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77c2a-130">Parameter</span></span>|<span data-ttu-id="77c2a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77c2a-131">Type</span></span>|<span data-ttu-id="77c2a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77c2a-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="77c2a-133">decision</span><span class="sxs-lookup"><span data-stu-id="77c2a-133">decision</span></span>  | <span data-ttu-id="77c2a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77c2a-134">String</span></span> | <span data-ttu-id="77c2a-135">Decisão de acesso para a entidade que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="77c2a-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="77c2a-136">Os valores possíveis são: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="77c2a-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="77c2a-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77c2a-137">Required.</span></span>  |
|  <span data-ttu-id="77c2a-138">justification</span><span class="sxs-lookup"><span data-stu-id="77c2a-138">justification</span></span> | <span data-ttu-id="77c2a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77c2a-139">String</span></span> | <span data-ttu-id="77c2a-140">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="77c2a-140">Context of the review provided to admins.</span></span> <span data-ttu-id="77c2a-141">Obrigatório se **justificationRequiredOnApproval** `True` estiver no **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="77c2a-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="77c2a-142">principalId</span><span class="sxs-lookup"><span data-stu-id="77c2a-142">principalId</span></span>|<span data-ttu-id="77c2a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77c2a-143">String</span></span>|<span data-ttu-id="77c2a-144">Se fornecido, todos os **accessReviewInstanceDecisionItems** com **principalId** correspondente serão revisados neste lote.</span><span class="sxs-lookup"><span data-stu-id="77c2a-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="77c2a-145">Se não for fornecido, todos os **principaisIds** serão revisados.</span><span class="sxs-lookup"><span data-stu-id="77c2a-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="77c2a-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="77c2a-146">resourceId</span></span>|<span data-ttu-id="77c2a-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77c2a-147">String</span></span>|<span data-ttu-id="77c2a-148">Se fornecido, todos os **accessReviewInstanceDecisionItems** com **resourceId** correspondentes serão revisados neste lote.</span><span class="sxs-lookup"><span data-stu-id="77c2a-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="77c2a-149">Se não for fornecido, todos **os resourceIds** serão revisados.</span><span class="sxs-lookup"><span data-stu-id="77c2a-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="77c2a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="77c2a-150">Response</span></span>

<span data-ttu-id="77c2a-151">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="77c2a-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="77c2a-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="77c2a-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77c2a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77c2a-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="77c2a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c2a-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json
Content-length: 113

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[<span data-ttu-id="77c2a-155">C#</span><span class="sxs-lookup"><span data-stu-id="77c2a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77c2a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c2a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c2a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c2a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77c2a-158">Java</span><span class="sxs-lookup"><span data-stu-id="77c2a-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="77c2a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="77c2a-159">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
