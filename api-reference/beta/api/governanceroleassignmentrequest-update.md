---
title: Atualizar governanceRoleAssignmentRequests
description: Permitir que os administradores atualizem suas`AdminApproved` decisões `AdminDenied`(ou) no governanceRoleAssignmentRequests que estão no `PendingAdminDecision`status de.
localization_priority: Normal
ms.openlocfilehash: 03f8d87d75a8edfa9c6b8fdc818114e0b41661ce
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440768"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="f87fd-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f87fd-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f87fd-104">Permitir que os administradores atualizem suas`AdminApproved` decisões `AdminDenied`(ou) no [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no `PendingAdminDecision`status de.</span><span class="sxs-lookup"><span data-stu-id="f87fd-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f87fd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87fd-105">Permissions</span></span>
<span data-ttu-id="f87fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f87fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f87fd-108">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de`owner` administrador `user access administrator`(ou) no recurso ao qual o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="f87fd-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="f87fd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f87fd-109">Permission type</span></span>      | <span data-ttu-id="f87fd-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87fd-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f87fd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f87fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f87fd-112">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f87fd-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f87fd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f87fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87fd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87fd-114">Not supported.</span></span>    |
|<span data-ttu-id="f87fd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f87fd-115">Application</span></span> | <span data-ttu-id="f87fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87fd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f87fd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f87fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="f87fd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f87fd-118">Request headers</span></span>
| <span data-ttu-id="f87fd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f87fd-119">Name</span></span>           | <span data-ttu-id="f87fd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f87fd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f87fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f87fd-121">Authorization</span></span>  | <span data-ttu-id="f87fd-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f87fd-122">Bearer {code}</span></span>|
| <span data-ttu-id="f87fd-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="f87fd-123">Content-type</span></span>  | <span data-ttu-id="f87fd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f87fd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f87fd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f87fd-125">Request body</span></span>

|<span data-ttu-id="f87fd-126">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="f87fd-126">Parameters</span></span>      |<span data-ttu-id="f87fd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f87fd-127">Type</span></span>                   |<span data-ttu-id="f87fd-128">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f87fd-128">Required</span></span> |<span data-ttu-id="f87fd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f87fd-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="f87fd-130">motivos</span><span class="sxs-lookup"><span data-stu-id="f87fd-130">reason</span></span>        |<span data-ttu-id="f87fd-131">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-131">String</span></span>                 |<span data-ttu-id="f87fd-132">✓</span><span class="sxs-lookup"><span data-stu-id="f87fd-132">✓</span></span>        |<span data-ttu-id="f87fd-133">O motivo fornecido pelo administrador para sua decisão.</span><span class="sxs-lookup"><span data-stu-id="f87fd-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="f87fd-134">sobre</span><span class="sxs-lookup"><span data-stu-id="f87fd-134">decision</span></span>        |<span data-ttu-id="f87fd-135">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-135">String</span></span>                 |<span data-ttu-id="f87fd-136">✓</span><span class="sxs-lookup"><span data-stu-id="f87fd-136">✓</span></span>        |<span data-ttu-id="f87fd-137">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f87fd-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="f87fd-138">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="f87fd-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="f87fd-139">Cronograma</span><span class="sxs-lookup"><span data-stu-id="f87fd-139">schedule</span></span>      |[<span data-ttu-id="f87fd-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f87fd-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="f87fd-141">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f87fd-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="f87fd-142">Para o status `AdminApproved`de, é necessário.</span><span class="sxs-lookup"><span data-stu-id="f87fd-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="f87fd-143">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="f87fd-143">assignmentState</span></span>      |<span data-ttu-id="f87fd-144">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-144">String</span></span>|         | <span data-ttu-id="f87fd-145">O estado da atribuição e os valores podem ser `Eligible` ou. `Active`</span><span class="sxs-lookup"><span data-stu-id="f87fd-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="f87fd-146">Para a decisão `AdminApproved`de, é necessário.</span><span class="sxs-lookup"><span data-stu-id="f87fd-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="f87fd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87fd-147">Response</span></span>
<span data-ttu-id="f87fd-148">Este método só pode ser aplicado a solicitações que estão no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="f87fd-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="f87fd-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f87fd-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f87fd-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f87fd-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f87fd-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f87fd-152">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f87fd-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f87fd-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f87fd-154">C#</span><span class="sxs-lookup"><span data-stu-id="f87fd-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f87fd-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="f87fd-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f87fd-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f87fd-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="f87fd-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f87fd-157">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="f87fd-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87fd-158">Response</span></span>
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
