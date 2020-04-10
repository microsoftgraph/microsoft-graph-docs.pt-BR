---
title: Atualizar governanceRoleAssignmentRequests
description: Permitir que os administradores atualizem suas`AdminApproved` decisões `AdminDenied`(ou) no governanceRoleAssignmentRequests que estão no `PendingAdminDecision`status de.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b726903082d8a3302e2be386206b76d741d89928
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218861"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="a2710-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a2710-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="a2710-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2710-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2710-105">Permitir que os administradores atualizem suas`AdminApproved` decisões `AdminDenied`(ou) no [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no `PendingAdminDecision`status de.</span><span class="sxs-lookup"><span data-stu-id="a2710-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2710-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2710-106">Permissions</span></span>
<span data-ttu-id="a2710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="a2710-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de`owner` administrador `user access administrator`(ou) no recurso ao qual o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="a2710-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="a2710-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2710-110">Permission type</span></span>      | <span data-ttu-id="a2710-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2710-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2710-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2710-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2710-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a2710-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a2710-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2710-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2710-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2710-115">Not supported.</span></span>    |
|<span data-ttu-id="a2710-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2710-116">Application</span></span> | <span data-ttu-id="a2710-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2710-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2710-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2710-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="a2710-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2710-119">Request headers</span></span>
| <span data-ttu-id="a2710-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a2710-120">Name</span></span>           | <span data-ttu-id="a2710-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2710-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2710-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2710-122">Authorization</span></span>  | <span data-ttu-id="a2710-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a2710-123">Bearer {code}</span></span>|
| <span data-ttu-id="a2710-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a2710-124">Content-type</span></span>  | <span data-ttu-id="a2710-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2710-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2710-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2710-126">Request body</span></span>

|<span data-ttu-id="a2710-127">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="a2710-127">Parameters</span></span>      |<span data-ttu-id="a2710-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2710-128">Type</span></span>                   |<span data-ttu-id="a2710-129">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a2710-129">Required</span></span> |<span data-ttu-id="a2710-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2710-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="a2710-131">motivo</span><span class="sxs-lookup"><span data-stu-id="a2710-131">reason</span></span>        |<span data-ttu-id="a2710-132">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a2710-132">String</span></span>                 |<span data-ttu-id="a2710-133">✓</span><span class="sxs-lookup"><span data-stu-id="a2710-133">✓</span></span>        |<span data-ttu-id="a2710-134">O motivo fornecido pelo administrador para sua decisão.</span><span class="sxs-lookup"><span data-stu-id="a2710-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="a2710-135">sobre</span><span class="sxs-lookup"><span data-stu-id="a2710-135">decision</span></span>        |<span data-ttu-id="a2710-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a2710-136">String</span></span>                 |<span data-ttu-id="a2710-137">✓</span><span class="sxs-lookup"><span data-stu-id="a2710-137">✓</span></span>        |<span data-ttu-id="a2710-138">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a2710-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="a2710-139">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="a2710-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="a2710-140">Cronograma</span><span class="sxs-lookup"><span data-stu-id="a2710-140">schedule</span></span>      |[<span data-ttu-id="a2710-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a2710-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="a2710-142">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a2710-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="a2710-143">Para o status `AdminApproved`de, é necessário.</span><span class="sxs-lookup"><span data-stu-id="a2710-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="a2710-144">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="a2710-144">assignmentState</span></span>      |<span data-ttu-id="a2710-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a2710-145">String</span></span>|         | <span data-ttu-id="a2710-146">O estado da atribuição e os valores podem ser `Eligible` ou. `Active`</span><span class="sxs-lookup"><span data-stu-id="a2710-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="a2710-147">Para a decisão `AdminApproved`de, é necessário.</span><span class="sxs-lookup"><span data-stu-id="a2710-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="a2710-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2710-148">Response</span></span>
<span data-ttu-id="a2710-149">Este método só pode ser aplicado a solicitações que estão no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="a2710-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="a2710-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2710-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2710-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2710-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2710-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2710-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a2710-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2710-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="a2710-155">C#</span><span class="sxs-lookup"><span data-stu-id="a2710-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2710-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2710-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2710-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2710-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="a2710-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2710-158">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="a2710-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2710-159">Response</span></span>
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
