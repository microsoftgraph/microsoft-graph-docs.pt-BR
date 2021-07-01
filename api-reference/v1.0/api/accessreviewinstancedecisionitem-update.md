---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize as propriedades de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ca2f5c24f10bd287b73502ec3d8ba5b6c399da18
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209608"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="8a279-103">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="8a279-103">Update accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="8a279-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a279-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a279-105">Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="8a279-105">Update the properties of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="8a279-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a279-106">Permissions</span></span>
<span data-ttu-id="8a279-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a279-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a279-109">Permission type</span></span>|<span data-ttu-id="8a279-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a279-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a279-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a279-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a279-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a279-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="8a279-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a279-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a279-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a279-114">Not supported.</span></span>|
|<span data-ttu-id="8a279-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a279-115">Application</span></span>|<span data-ttu-id="8a279-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a279-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="8a279-117">Somente um usuário de chamada listado como revisor do [accessReviewInstance](../resources/accessreviewinstance.md) pai pode atualizar **o accessReviewInstanceDecisionItem**.</span><span class="sxs-lookup"><span data-stu-id="8a279-117">Only a calling user who is listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md) can update the **accessReviewInstanceDecisionItem**.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a279-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a279-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="8a279-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a279-119">Request headers</span></span>
|<span data-ttu-id="8a279-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8a279-120">Name</span></span>|<span data-ttu-id="8a279-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a279-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a279-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a279-122">Authorization</span></span>|<span data-ttu-id="8a279-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a279-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a279-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a279-125">Content-Type</span></span>|<span data-ttu-id="8a279-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a279-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a279-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a279-128">Request body</span></span>
<span data-ttu-id="8a279-129">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="8a279-129">In the request body, supply a JSON representation of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

<span data-ttu-id="8a279-130">A tabela a seguir mostra as propriedades que são aceitas quando você atualiza [o accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="8a279-130">The following table shows the properties that are accepted when you update the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

|<span data-ttu-id="8a279-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a279-131">Property</span></span>|<span data-ttu-id="8a279-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a279-132">Type</span></span>|<span data-ttu-id="8a279-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a279-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a279-134">decision</span><span class="sxs-lookup"><span data-stu-id="8a279-134">decision</span></span>|<span data-ttu-id="8a279-135">String</span><span class="sxs-lookup"><span data-stu-id="8a279-135">String</span></span>|<span data-ttu-id="8a279-136">O voto do revistor sobre se a entidade deve ter acesso ao recurso em revisão.</span><span class="sxs-lookup"><span data-stu-id="8a279-136">The reviewer's vote on whether the principal should have access to the resource under review.</span></span> <span data-ttu-id="8a279-137">Valores possíveis: `Approve` `Deny` , ou `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="8a279-137">Possible values: `Approve`, `Deny`, or `DontKnow`.</span></span> <span data-ttu-id="8a279-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a279-138">Required.</span></span>|
|<span data-ttu-id="8a279-139">justification</span><span class="sxs-lookup"><span data-stu-id="8a279-139">justification</span></span>|<span data-ttu-id="8a279-140">String</span><span class="sxs-lookup"><span data-stu-id="8a279-140">String</span></span>|<span data-ttu-id="8a279-141">O motivo da decisão do revistor.</span><span class="sxs-lookup"><span data-stu-id="8a279-141">The reviewer's reason for decision.</span></span> <span data-ttu-id="8a279-142">Obrigatório se a **justificationRequiredOnApproval** da propriedade settings do [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) for `true` .</span><span class="sxs-lookup"><span data-stu-id="8a279-142">Required if the **justificationRequiredOnApproval** of the settings property of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="8a279-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a279-143">Response</span></span>

<span data-ttu-id="8a279-144">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="8a279-144">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8a279-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8a279-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a279-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a279-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8a279-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a279-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8a279-148">C#</span><span class="sxs-lookup"><span data-stu-id="8a279-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a279-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a279-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a279-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a279-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a279-151">Java</span><span class="sxs-lookup"><span data-stu-id="8a279-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8a279-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a279-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
