---
title: Cancelar privilegedRoleAssignmentRequest
description: Cancelar uma privilegedRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: acf272e1368b89b5112d7fd96ab6d0944a717552
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361020"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="dd9bb-103">Cancelar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="dd9bb-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd9bb-104">Cancelar uma [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="dd9bb-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd9bb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd9bb-105">Permissions</span></span>
<span data-ttu-id="dd9bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd9bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd9bb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd9bb-108">Permission type</span></span>                        | <span data-ttu-id="dd9bb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd9bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd9bb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd9bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd9bb-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="dd9bb-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd9bb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd9bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd9bb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-113">Not supported.</span></span> |
|<span data-ttu-id="dd9bb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd9bb-114">Application</span></span>                            | <span data-ttu-id="dd9bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="dd9bb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd9bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="dd9bb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd9bb-117">Request headers</span></span>
| <span data-ttu-id="dd9bb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="dd9bb-118">Name</span></span>      |<span data-ttu-id="dd9bb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd9bb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd9bb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd9bb-120">Authorization</span></span>  | <span data-ttu-id="dd9bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd9bb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd9bb-123">Request body</span></span>
<span data-ttu-id="dd9bb-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd9bb-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd9bb-125">Response</span></span>
<span data-ttu-id="dd9bb-126">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="dd9bb-127">Ele retorna [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="dd9bb-128">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="dd9bb-128">Error codes</span></span>
<span data-ttu-id="dd9bb-129">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="dd9bb-130">Além disso, ele retorna os códigos de erro personalizados listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="dd9bb-131">Código de erro</span><span class="sxs-lookup"><span data-stu-id="dd9bb-131">Error code</span></span>     | <span data-ttu-id="dd9bb-132">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="dd9bb-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="dd9bb-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd9bb-133">400 BadRequest</span></span> | <span data-ttu-id="dd9bb-134">RequestId não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="dd9bb-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd9bb-135">400 BadRequest</span></span> | <span data-ttu-id="dd9bb-136">Solicitação com ID de solicitação não encontrada.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="dd9bb-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd9bb-137">400 BadRequest</span></span> | <span data-ttu-id="dd9bb-138">O cancelamento pode ser feito apenas em status agendado e PendingApproval.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="dd9bb-139">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="dd9bb-139">403 UnAuthorized</span></span> | <span data-ttu-id="dd9bb-140">O solicitante não tem permissão para cancelar a chamada ou a solicitação de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="dd9bb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd9bb-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd9bb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd9bb-142">Request</span></span>
<span data-ttu-id="dd9bb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd9bb-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd9bb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd9bb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd9bb-145">C#</span><span class="sxs-lookup"><span data-stu-id="dd9bb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-privilegedroleassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd9bb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd9bb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-privilegedroleassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd9bb-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dd9bb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-privilegedroleassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd9bb-148">Java</span><span class="sxs-lookup"><span data-stu-id="dd9bb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-privilegedroleassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd9bb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd9bb-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
