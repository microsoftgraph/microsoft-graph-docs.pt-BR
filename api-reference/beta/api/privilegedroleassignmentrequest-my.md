---
title: 'privilegedRoleAssignmentRequest: My'
description: Obtenha as solicitações de atribuição de função privilegiada do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 0954dab90dd43f4afdc6ed384ec8e2f540cc1dd0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034949"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="8388f-103">privilegedRoleAssignmentRequest: My</span><span class="sxs-lookup"><span data-stu-id="8388f-103">privilegedRoleAssignmentRequest: my</span></span>

<span data-ttu-id="8388f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8388f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8388f-105">Obtenha as solicitações de atribuição de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="8388f-105">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="8388f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8388f-106">Permissions</span></span>
<span data-ttu-id="8388f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8388f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8388f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8388f-109">Permission type</span></span>                        | <span data-ttu-id="8388f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8388f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8388f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8388f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8388f-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="8388f-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8388f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8388f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8388f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8388f-114">Not supported.</span></span> |
|<span data-ttu-id="8388f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8388f-115">Application</span></span>                            | <span data-ttu-id="8388f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8388f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8388f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8388f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8388f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8388f-118">Optional query parameters</span></span>
<span data-ttu-id="8388f-119">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8388f-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8388f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8388f-120">Request headers</span></span>
| <span data-ttu-id="8388f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8388f-121">Name</span></span>      |<span data-ttu-id="8388f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8388f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8388f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8388f-123">Authorization</span></span>  | <span data-ttu-id="8388f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8388f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8388f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8388f-126">Request body</span></span>
<span data-ttu-id="8388f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8388f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8388f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8388f-128">Response</span></span>
<span data-ttu-id="8388f-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8388f-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8388f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8388f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8388f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8388f-131">Request</span></span>
<span data-ttu-id="8388f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8388f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8388f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8388f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="c"></a>[<span data-ttu-id="8388f-134">C#</span><span class="sxs-lookup"><span data-stu-id="8388f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8388f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8388f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8388f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8388f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8388f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8388f-137">Response</span></span>
<span data-ttu-id="8388f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8388f-138">The following is an example of the response.</span></span> <span data-ttu-id="8388f-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8388f-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8388f-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8388f-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
    "@odata.count": 4,
    "value": [{
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-08T02:35:17.903Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
         "userId": "Self",
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
        "status": "RequestedApproval",
        "duration": "2",
        "reason": "Activate the role for business purpose",
        "ticketNumber": "234",
        "ticketSystem": "system",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }, {
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-07T22:55:00Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "03ea0c3d-90a0-42d4-b220-11c049c506fb",
        "userId": "Self",
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-07T22:17:37.2215343Z",
        "status": "ApprovalAborted",
        "duration": "1",
        "reason": "Activate for testing",
        "ticketNumber": "222",
        "ticketSystem": "222",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('03ea0c3d-90a0-42d4-b220-11c049c506fb')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


