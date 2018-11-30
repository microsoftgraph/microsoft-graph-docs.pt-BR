---
title: Cancelar privilegedRoleAssignmentRequest
description: Cancele um privilegedRoleAssignmentRequest.
ms.openlocfilehash: 99c1102235e93ca365dcdd0e619bcceac9f396f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037867"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="372da-103">Cancelar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="372da-103">Cancel privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="372da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="372da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="372da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="372da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="372da-106">Cancele um [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="372da-106">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="372da-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="372da-107">Permissions</span></span>
<span data-ttu-id="372da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="372da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="372da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="372da-110">Permission type</span></span>                        | <span data-ttu-id="372da-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="372da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="372da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="372da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="372da-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="372da-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="372da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="372da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="372da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="372da-115">Not supported.</span></span> |
|<span data-ttu-id="372da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="372da-116">Application</span></span>                            | <span data-ttu-id="372da-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="372da-117">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="372da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="372da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="372da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="372da-119">Request headers</span></span>
| <span data-ttu-id="372da-120">Nome</span><span class="sxs-lookup"><span data-stu-id="372da-120">Name</span></span>      |<span data-ttu-id="372da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="372da-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="372da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="372da-122">Authorization</span></span>  | <span data-ttu-id="372da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="372da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="372da-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="372da-125">Request body</span></span>
<span data-ttu-id="372da-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="372da-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="372da-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="372da-127">Response</span></span>
<span data-ttu-id="372da-128">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="372da-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="372da-129">Ele retorna [privilegedRoleAssignmentRequest] (… / resources/privilegedRoleAssignmentRequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="372da-129">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="372da-130">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="372da-130">Error codes</span></span>
<span data-ttu-id="372da-131">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="372da-131">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="372da-132">Além disso, ele retorna os códigos de erro personalizado listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="372da-132">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="372da-133">Código de erro</span><span class="sxs-lookup"><span data-stu-id="372da-133">Error code</span></span>     | <span data-ttu-id="372da-134">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="372da-134">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="372da-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="372da-135">400 BadRequest</span></span> | <span data-ttu-id="372da-136">RequestId não pode ser Null.</span><span class="sxs-lookup"><span data-stu-id="372da-136">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="372da-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="372da-137">400 BadRequest</span></span> | <span data-ttu-id="372da-138">Solicitar com ID de solicitação não encontrado.</span><span class="sxs-lookup"><span data-stu-id="372da-138">Request with request ID not found.</span></span> |
| <span data-ttu-id="372da-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="372da-139">400 BadRequest</span></span> | <span data-ttu-id="372da-140">Cancelamento pode ser feito somente em status agendadas e PendingApproval.</span><span class="sxs-lookup"><span data-stu-id="372da-140">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="372da-141">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="372da-141">403 UnAuthorized</span></span> | <span data-ttu-id="372da-142">Solicitante não pode fazer a chamada de cancelar ou solicitação não encontrado.</span><span class="sxs-lookup"><span data-stu-id="372da-142">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="372da-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="372da-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="372da-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="372da-144">Request</span></span>
<span data-ttu-id="372da-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="372da-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="372da-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="372da-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequests"
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
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
