---
title: Atualizar governanceRoleAssignmentRequests
description: Permitir que os administradores atualizem suas`AdminApproved` decisões `AdminDenied`(ou) no governanceRoleAssignmentRequests que estão no `PendingAdminDecision`status de.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: d8fc97ff329b171050b0309161ec818a9996d4ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420945"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="1b599-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="1b599-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="1b599-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1b599-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b599-105">Permitir que os administradores atualizem suas`AdminApproved` decisões `AdminDenied`(ou) no [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no `PendingAdminDecision`status de.</span><span class="sxs-lookup"><span data-stu-id="1b599-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b599-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b599-106">Permissions</span></span>
<span data-ttu-id="1b599-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="1b599-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de`owner` administrador `user access administrator`(ou) no recurso ao qual o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="1b599-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="1b599-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b599-110">Permission type</span></span>      | <span data-ttu-id="1b599-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b599-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b599-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b599-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b599-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1b599-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="1b599-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b599-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b599-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b599-115">Not supported.</span></span>    |
|<span data-ttu-id="1b599-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b599-116">Application</span></span> | <span data-ttu-id="1b599-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b599-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b599-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b599-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="1b599-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b599-119">Request headers</span></span>
| <span data-ttu-id="1b599-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1b599-120">Name</span></span>           | <span data-ttu-id="1b599-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b599-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1b599-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b599-122">Authorization</span></span>  | <span data-ttu-id="1b599-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1b599-123">Bearer {code}</span></span>|
| <span data-ttu-id="1b599-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1b599-124">Content-type</span></span>  | <span data-ttu-id="1b599-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b599-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b599-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b599-126">Request body</span></span>

|<span data-ttu-id="1b599-127">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="1b599-127">Parameters</span></span>      |<span data-ttu-id="1b599-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b599-128">Type</span></span>                   |<span data-ttu-id="1b599-129">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="1b599-129">Required</span></span> |<span data-ttu-id="1b599-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b599-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="1b599-131">motivo</span><span class="sxs-lookup"><span data-stu-id="1b599-131">reason</span></span>        |<span data-ttu-id="1b599-132">String</span><span class="sxs-lookup"><span data-stu-id="1b599-132">String</span></span>                 |<span data-ttu-id="1b599-133">✓</span><span class="sxs-lookup"><span data-stu-id="1b599-133">✓</span></span>        |<span data-ttu-id="1b599-134">O motivo fornecido pelo administrador para sua decisão.</span><span class="sxs-lookup"><span data-stu-id="1b599-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="1b599-135">sobre</span><span class="sxs-lookup"><span data-stu-id="1b599-135">decision</span></span>        |<span data-ttu-id="1b599-136">String</span><span class="sxs-lookup"><span data-stu-id="1b599-136">String</span></span>                 |<span data-ttu-id="1b599-137">✓</span><span class="sxs-lookup"><span data-stu-id="1b599-137">✓</span></span>        |<span data-ttu-id="1b599-138">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1b599-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="1b599-139">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="1b599-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="1b599-140">Cronograma</span><span class="sxs-lookup"><span data-stu-id="1b599-140">schedule</span></span>      |[<span data-ttu-id="1b599-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="1b599-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="1b599-142">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1b599-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="1b599-143">Para o status `AdminApproved`de, é necessário.</span><span class="sxs-lookup"><span data-stu-id="1b599-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="1b599-144">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="1b599-144">assignmentState</span></span>      |<span data-ttu-id="1b599-145">String</span><span class="sxs-lookup"><span data-stu-id="1b599-145">String</span></span>|         | <span data-ttu-id="1b599-146">O estado da atribuição e os valores podem ser `Eligible` ou. `Active`</span><span class="sxs-lookup"><span data-stu-id="1b599-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="1b599-147">Para a decisão `AdminApproved`de, é necessário.</span><span class="sxs-lookup"><span data-stu-id="1b599-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="1b599-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b599-148">Response</span></span>
<span data-ttu-id="1b599-149">Este método só pode ser aplicado a solicitações que estão no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="1b599-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="1b599-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b599-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b599-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b599-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b599-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b599-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1b599-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b599-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="1b599-155">C#</span><span class="sxs-lookup"><span data-stu-id="1b599-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b599-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b599-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b599-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b599-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="1b599-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b599-158">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="1b599-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b599-159">Response</span></span>
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
