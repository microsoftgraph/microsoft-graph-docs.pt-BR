---
title: Atualizar governanceRoleAssignmentRequests
description: Permitem que administradores atualizar suas decisões (`AdminApproved` ou `AdminDenied`) em governanceRoleAssignmentRequests que estão no status de `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 3d68e06688922177e2a1a183a9fe4bfc6be6a91d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874932"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="fd6e7-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="fd6e7-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="fd6e7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd6e7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd6e7-106">Permitem que administradores atualizar suas decisões (`AdminApproved` ou `AdminDenied`) em [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd6e7-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd6e7-107">Permissions</span></span>
<span data-ttu-id="fd6e7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd6e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="fd6e7-110">**Observação:** Essa API também requer que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) em relação ao qual pertence o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) recurso.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-110">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="fd6e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd6e7-111">Permission type</span></span>      | <span data-ttu-id="fd6e7-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd6e7-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd6e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd6e7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fd6e7-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="fd6e7-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="fd6e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd6e7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd6e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-116">Not supported.</span></span>    |
|<span data-ttu-id="fd6e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd6e7-117">Application</span></span> | <span data-ttu-id="fd6e7-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="fd6e7-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd6e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd6e7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="fd6e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6e7-120">Request headers</span></span>
| <span data-ttu-id="fd6e7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fd6e7-121">Name</span></span>           | <span data-ttu-id="fd6e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd6e7-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd6e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd6e7-123">Authorization</span></span>  | <span data-ttu-id="fd6e7-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="fd6e7-124">Bearer {code}</span></span>|
| <span data-ttu-id="fd6e7-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="fd6e7-125">Content-type</span></span>  | <span data-ttu-id="fd6e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd6e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd6e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6e7-127">Request body</span></span>

|<span data-ttu-id="fd6e7-128">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="fd6e7-128">Parameters</span></span>      |<span data-ttu-id="fd6e7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd6e7-129">Type</span></span>                   |<span data-ttu-id="fd6e7-130">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="fd6e7-130">Required</span></span> |<span data-ttu-id="fd6e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd6e7-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="fd6e7-132">motivo</span><span class="sxs-lookup"><span data-stu-id="fd6e7-132">reason</span></span>        |<span data-ttu-id="fd6e7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd6e7-133">String</span></span>                 |<span data-ttu-id="fd6e7-134">✓</span><span class="sxs-lookup"><span data-stu-id="fd6e7-134">✓</span></span>        |<span data-ttu-id="fd6e7-135">O motivo fornecido pelo administrador para a sua decisão.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="fd6e7-136">decisão</span><span class="sxs-lookup"><span data-stu-id="fd6e7-136">decision</span></span>        |<span data-ttu-id="fd6e7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd6e7-137">String</span></span>                 |<span data-ttu-id="fd6e7-138">✓</span><span class="sxs-lookup"><span data-stu-id="fd6e7-138">✓</span></span>        |<span data-ttu-id="fd6e7-139">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="fd6e7-140">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="fd6e7-141">agenda</span><span class="sxs-lookup"><span data-stu-id="fd6e7-141">schedule</span></span>      |[<span data-ttu-id="fd6e7-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fd6e7-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="fd6e7-143">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="fd6e7-144">Status da `AdminApproved`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="fd6e7-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fd6e7-145">assignmentState</span></span>      |<span data-ttu-id="fd6e7-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd6e7-146">String</span></span>|         | <span data-ttu-id="fd6e7-147">O estado da atribuição e os valores pode ser `Eligible` ou `Active`.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="fd6e7-148">Decisão de `AdminApproved`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="fd6e7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd6e7-149">Response</span></span>
<span data-ttu-id="fd6e7-150">Esse método só pode ser aplicado a solicitações que estejam no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="fd6e7-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd6e7-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd6e7-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd6e7-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd6e7-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6e7-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="fd6e7-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd6e7-155">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="fd6e7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd6e7-156">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
