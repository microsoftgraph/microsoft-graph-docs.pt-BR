---
title: Atualizar governanceRoleAssignmentRequests
description: Permitir que os administradores atualizem suas decisões ( `AdminApproved` ou `AdminDenied` ) no governanceRoleAssignmentRequests que estão no status de `PendingAdminDecision` .
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 95ff7dbf174a5dc6287be0fc7476c21596e651ba
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634857"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="5d7b6-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="5d7b6-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="5d7b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d7b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d7b6-105">Permitir que os administradores atualizem suas decisões ( `AdminApproved` ou `AdminDenied` ) no [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="5d7b6-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d7b6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d7b6-106">Permissions</span></span>
<span data-ttu-id="5d7b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="5d7b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="5d7b6-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador ( `owner` ou `user access administrator` ) no recurso ao qual o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

### <a name="azure-resources"></a><span data-ttu-id="5d7b6-110">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="5d7b6-110">Azure resources</span></span>

| <span data-ttu-id="5d7b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d7b6-111">Permission type</span></span> | <span data-ttu-id="5d7b6-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d7b6-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="5d7b6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d7b6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5d7b6-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="5d7b6-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="5d7b6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d7b6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-116">Not supported.</span></span> |
| <span data-ttu-id="5d7b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d7b6-117">Application</span></span> | <span data-ttu-id="5d7b6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="5d7b6-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="5d7b6-119">Azure AD</span></span>

| <span data-ttu-id="5d7b6-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d7b6-120">Permission type</span></span> | <span data-ttu-id="5d7b6-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d7b6-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="5d7b6-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d7b6-122">Delegated (work or school account)</span></span> | <span data-ttu-id="5d7b6-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="5d7b6-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="5d7b6-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d7b6-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7b6-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-125">Not supported.</span></span> |
| <span data-ttu-id="5d7b6-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d7b6-126">Application</span></span> | <span data-ttu-id="5d7b6-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="5d7b6-128">Grupos</span><span class="sxs-lookup"><span data-stu-id="5d7b6-128">Groups</span></span>

|<span data-ttu-id="5d7b6-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d7b6-129">Permission type</span></span> | <span data-ttu-id="5d7b6-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d7b6-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="5d7b6-131">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d7b6-131">Delegated (work or school account)</span></span> | <span data-ttu-id="5d7b6-132">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="5d7b6-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="5d7b6-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d7b6-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7b6-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-134">Not supported.</span></span> |
| <span data-ttu-id="5d7b6-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d7b6-135">Application</span></span> | <span data-ttu-id="5d7b6-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d7b6-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d7b6-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="5d7b6-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7b6-138">Request headers</span></span>
| <span data-ttu-id="5d7b6-139">Nome</span><span class="sxs-lookup"><span data-stu-id="5d7b6-139">Name</span></span>           | <span data-ttu-id="5d7b6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d7b6-140">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d7b6-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d7b6-141">Authorization</span></span>  | <span data-ttu-id="5d7b6-142">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5d7b6-142">Bearer {code}</span></span>|
| <span data-ttu-id="5d7b6-143">Content-type</span><span class="sxs-lookup"><span data-stu-id="5d7b6-143">Content-type</span></span>  | <span data-ttu-id="5d7b6-144">application/json</span><span class="sxs-lookup"><span data-stu-id="5d7b6-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d7b6-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7b6-145">Request body</span></span>

|<span data-ttu-id="5d7b6-146">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="5d7b6-146">Parameters</span></span>      |<span data-ttu-id="5d7b6-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d7b6-147">Type</span></span>                   |<span data-ttu-id="5d7b6-148">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="5d7b6-148">Required</span></span> |<span data-ttu-id="5d7b6-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d7b6-149">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="5d7b6-150">motivo</span><span class="sxs-lookup"><span data-stu-id="5d7b6-150">reason</span></span>        |<span data-ttu-id="5d7b6-151">String</span><span class="sxs-lookup"><span data-stu-id="5d7b6-151">String</span></span>                 |<span data-ttu-id="5d7b6-152">✓</span><span class="sxs-lookup"><span data-stu-id="5d7b6-152">✓</span></span>        |<span data-ttu-id="5d7b6-153">O motivo fornecido pelo administrador para sua decisão.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-153">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="5d7b6-154">sobre</span><span class="sxs-lookup"><span data-stu-id="5d7b6-154">decision</span></span>        |<span data-ttu-id="5d7b6-155">String</span><span class="sxs-lookup"><span data-stu-id="5d7b6-155">String</span></span>                 |<span data-ttu-id="5d7b6-156">✓</span><span class="sxs-lookup"><span data-stu-id="5d7b6-156">✓</span></span>        |<span data-ttu-id="5d7b6-157">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-157">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="5d7b6-158">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied` .</span><span class="sxs-lookup"><span data-stu-id="5d7b6-158">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="5d7b6-159">Cronograma</span><span class="sxs-lookup"><span data-stu-id="5d7b6-159">schedule</span></span>      |[<span data-ttu-id="5d7b6-160">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5d7b6-160">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="5d7b6-161">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-161">The schedule of the role assignment request.</span></span> <span data-ttu-id="5d7b6-162">Para o status de `AdminApproved` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-162">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="5d7b6-163">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="5d7b6-163">assignmentState</span></span>      |<span data-ttu-id="5d7b6-164">String</span><span class="sxs-lookup"><span data-stu-id="5d7b6-164">String</span></span>|         | <span data-ttu-id="5d7b6-165">O estado da atribuição e os valores podem ser `Eligible` ou `Active` .</span><span class="sxs-lookup"><span data-stu-id="5d7b6-165">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="5d7b6-166">Para a decisão de `AdminApproved` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-166">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="5d7b6-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d7b6-167">Response</span></span>
<span data-ttu-id="5d7b6-168">Este método só pode ser aplicado a solicitações que estão no status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="5d7b6-168">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="5d7b6-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d7b6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d7b6-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d7b6-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d7b6-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7b6-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d7b6-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d7b6-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="5d7b6-174">C#</span><span class="sxs-lookup"><span data-stu-id="5d7b6-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d7b6-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d7b6-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d7b6-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d7b6-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="5d7b6-177">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7b6-177">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="5d7b6-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d7b6-178">Response</span></span>
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


