---
title: Atualizar governançaRoleAssignmentRequests
description: Permitir que os administradores atualizem suas decisões ( ou ) sobre `AdminApproved` `AdminDenied` governançaRoleAssignmentRequests que estão em status de `PendingAdminDecision` .
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 59080cf19cf96d82f029d3ba9513cd16a042157a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435851"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="157a3-103">Atualizar governançaRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="157a3-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="157a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="157a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="157a3-105">Permitir que os administradores atualizem suas decisões ( ou ) sobre `AdminApproved` `AdminDenied` [governançaRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão em status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="157a3-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="157a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="157a3-106">Permissions</span></span>
<span data-ttu-id="157a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="157a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="157a3-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função de administrador ( ou ) no recurso ao qual a `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="157a3-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

### <a name="azure-resources"></a><span data-ttu-id="157a3-110">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="157a3-110">Azure resources</span></span>

| <span data-ttu-id="157a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="157a3-111">Permission type</span></span> | <span data-ttu-id="157a3-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="157a3-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="157a3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="157a3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="157a3-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="157a3-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="157a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="157a3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="157a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="157a3-116">Not supported.</span></span> |
| <span data-ttu-id="157a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="157a3-117">Application</span></span> | <span data-ttu-id="157a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="157a3-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="157a3-119">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="157a3-119">Azure AD</span></span>

| <span data-ttu-id="157a3-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="157a3-120">Permission type</span></span> | <span data-ttu-id="157a3-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="157a3-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="157a3-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="157a3-122">Delegated (work or school account)</span></span> | <span data-ttu-id="157a3-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="157a3-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="157a3-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="157a3-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="157a3-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="157a3-125">Not supported.</span></span> |
| <span data-ttu-id="157a3-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="157a3-126">Application</span></span> | <span data-ttu-id="157a3-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="157a3-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="157a3-128">Grupos</span><span class="sxs-lookup"><span data-stu-id="157a3-128">Groups</span></span>

|<span data-ttu-id="157a3-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="157a3-129">Permission type</span></span> | <span data-ttu-id="157a3-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="157a3-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="157a3-131">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="157a3-131">Delegated (work or school account)</span></span> | <span data-ttu-id="157a3-132">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="157a3-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="157a3-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="157a3-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="157a3-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="157a3-134">Not supported.</span></span> |
| <span data-ttu-id="157a3-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="157a3-135">Application</span></span> | <span data-ttu-id="157a3-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="157a3-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="157a3-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="157a3-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="157a3-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="157a3-138">Request headers</span></span>
| <span data-ttu-id="157a3-139">Nome</span><span class="sxs-lookup"><span data-stu-id="157a3-139">Name</span></span>           | <span data-ttu-id="157a3-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="157a3-140">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="157a3-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="157a3-141">Authorization</span></span>  | <span data-ttu-id="157a3-142">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="157a3-142">Bearer {code}</span></span>|
| <span data-ttu-id="157a3-143">Content-type</span><span class="sxs-lookup"><span data-stu-id="157a3-143">Content-type</span></span>  | <span data-ttu-id="157a3-144">application/json</span><span class="sxs-lookup"><span data-stu-id="157a3-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="157a3-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="157a3-145">Request body</span></span>

|<span data-ttu-id="157a3-146">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="157a3-146">Parameters</span></span>      |<span data-ttu-id="157a3-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="157a3-147">Type</span></span>                   |<span data-ttu-id="157a3-148">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="157a3-148">Required</span></span> |<span data-ttu-id="157a3-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="157a3-149">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="157a3-150">motivo</span><span class="sxs-lookup"><span data-stu-id="157a3-150">reason</span></span>        |<span data-ttu-id="157a3-151">String</span><span class="sxs-lookup"><span data-stu-id="157a3-151">String</span></span>                 |<span data-ttu-id="157a3-152">✓</span><span class="sxs-lookup"><span data-stu-id="157a3-152">✓</span></span>        |<span data-ttu-id="157a3-153">O motivo fornecido pelo administrador para sua decisão.</span><span class="sxs-lookup"><span data-stu-id="157a3-153">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="157a3-154">decision</span><span class="sxs-lookup"><span data-stu-id="157a3-154">decision</span></span>        |<span data-ttu-id="157a3-155">String</span><span class="sxs-lookup"><span data-stu-id="157a3-155">String</span></span>                 |<span data-ttu-id="157a3-156">✓</span><span class="sxs-lookup"><span data-stu-id="157a3-156">✓</span></span>        |<span data-ttu-id="157a3-157">A decisão do administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="157a3-157">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="157a3-158">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied` .</span><span class="sxs-lookup"><span data-stu-id="157a3-158">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="157a3-159">Cronograma</span><span class="sxs-lookup"><span data-stu-id="157a3-159">schedule</span></span>      |[<span data-ttu-id="157a3-160">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="157a3-160">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="157a3-161">O cronograma da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="157a3-161">The schedule of the role assignment request.</span></span> <span data-ttu-id="157a3-162">Para o status `AdminApproved` de , é necessário.</span><span class="sxs-lookup"><span data-stu-id="157a3-162">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="157a3-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="157a3-163">assignmentState</span></span>      |<span data-ttu-id="157a3-164">String</span><span class="sxs-lookup"><span data-stu-id="157a3-164">String</span></span>|         | <span data-ttu-id="157a3-165">O estado da atribuição e os valores podem `Eligible` ser ou `Active` .</span><span class="sxs-lookup"><span data-stu-id="157a3-165">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="157a3-166">Para a decisão `AdminApproved` de , é necessário.</span><span class="sxs-lookup"><span data-stu-id="157a3-166">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="157a3-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="157a3-167">Response</span></span>
<span data-ttu-id="157a3-168">Esse método só pode ser aplicado a solicitações que estão em status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="157a3-168">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="157a3-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="157a3-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="157a3-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="157a3-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="157a3-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="157a3-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="157a3-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="157a3-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="157a3-174">C#</span><span class="sxs-lookup"><span data-stu-id="157a3-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="157a3-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="157a3-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="157a3-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="157a3-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="157a3-177">Java</span><span class="sxs-lookup"><span data-stu-id="157a3-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updaterequest-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="157a3-178">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="157a3-178">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="157a3-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="157a3-179">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


