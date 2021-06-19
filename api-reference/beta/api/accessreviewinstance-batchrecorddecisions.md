---
title: 'accessReviewInstance: batchRecordDecisions'
description: Permite que os revisores revisem todos os objetos accessReviewInstanceDecisionItem em lotes.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ab7e7e3580275aa127bbb01e34484a823d4b01bf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030744"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="0b3c9-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="0b3c9-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="0b3c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b3c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b3c9-105">Permite que os revisores revisem todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em lotes usando **principalId,** **resourceId** ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b3c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b3c9-106">Permissions</span></span>
<span data-ttu-id="0b3c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b3c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b3c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b3c9-109">Permission type</span></span>|<span data-ttu-id="0b3c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b3c9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b3c9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b3c9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b3c9-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3c9-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="0b3c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b3c9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b3c9-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0b3c9-114">Not supported</span></span>|
|<span data-ttu-id="0b3c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b3c9-115">Application</span></span>|<span data-ttu-id="0b3c9-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b3c9-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b3c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b3c9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="0b3c9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b3c9-118">Request headers</span></span>
|<span data-ttu-id="0b3c9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0b3c9-119">Name</span></span>|<span data-ttu-id="0b3c9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b3c9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b3c9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b3c9-121">Authorization</span></span>|<span data-ttu-id="0b3c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0b3c9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b3c9-124">Content-Type</span></span>|<span data-ttu-id="0b3c9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b3c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b3c9-127">Request body</span></span>
<span data-ttu-id="0b3c9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0b3c9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0b3c9-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0b3c9-130">Parameter</span></span>|<span data-ttu-id="0b3c9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b3c9-131">Type</span></span>|<span data-ttu-id="0b3c9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b3c9-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="0b3c9-133">decision</span><span class="sxs-lookup"><span data-stu-id="0b3c9-133">decision</span></span>  | <span data-ttu-id="0b3c9-134">String</span><span class="sxs-lookup"><span data-stu-id="0b3c9-134">String</span></span> | <span data-ttu-id="0b3c9-135">Decisão de acesso para a entidade que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="0b3c9-136">Os valores possíveis são: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="0b3c9-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-137">Required.</span></span>  |
|  <span data-ttu-id="0b3c9-138">justification</span><span class="sxs-lookup"><span data-stu-id="0b3c9-138">justification</span></span> | <span data-ttu-id="0b3c9-139">String</span><span class="sxs-lookup"><span data-stu-id="0b3c9-139">String</span></span> | <span data-ttu-id="0b3c9-140">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-140">Context of the review provided to admins.</span></span> <span data-ttu-id="0b3c9-141">Obrigatório se **justificationRequiredOnApproval** `True` estiver no **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="0b3c9-142">principalId</span><span class="sxs-lookup"><span data-stu-id="0b3c9-142">principalId</span></span>|<span data-ttu-id="0b3c9-143">String</span><span class="sxs-lookup"><span data-stu-id="0b3c9-143">String</span></span>|<span data-ttu-id="0b3c9-144">Se fornecido, todos os **accessReviewInstanceDecisionItems** com **principalId** correspondente serão revisados neste lote.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="0b3c9-145">Se não for fornecido, todos os **principaisIds** serão revisados.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="0b3c9-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="0b3c9-146">resourceId</span></span>|<span data-ttu-id="0b3c9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b3c9-147">String</span></span>|<span data-ttu-id="0b3c9-148">Se fornecido, todos os **accessReviewInstanceDecisionItems** com **resourceId** correspondentes serão revisados neste lote.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="0b3c9-149">Se não for fornecido, todos **os resourceIds** serão revisados.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="0b3c9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b3c9-150">Response</span></span>

<span data-ttu-id="0b3c9-151">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b3c9-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0b3c9-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0b3c9-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b3c9-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b3c9-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0b3c9-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b3c9-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[<span data-ttu-id="0b3c9-155">C#</span><span class="sxs-lookup"><span data-stu-id="0b3c9-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b3c9-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b3c9-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b3c9-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b3c9-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b3c9-158">Java</span><span class="sxs-lookup"><span data-stu-id="0b3c9-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0b3c9-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b3c9-159">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
