---
title: 'privilegedRoleAssignmentRequest: My'
description: Obtenha as solicitações de atribuição de função privilegiada do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a597e5724122950cd5e66ffa3b383bf0c38e57fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455302"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="9e449-103">privilegedRoleAssignmentRequest: My</span><span class="sxs-lookup"><span data-stu-id="9e449-103">privilegedRoleAssignmentRequest: my</span></span>

<span data-ttu-id="9e449-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9e449-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e449-105">Obtenha as solicitações de atribuição de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="9e449-105">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e449-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e449-106">Permissions</span></span>
<span data-ttu-id="9e449-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e449-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e449-109">Permission type</span></span>                        | <span data-ttu-id="9e449-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e449-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e449-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e449-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9e449-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9e449-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e449-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e449-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e449-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e449-114">Not supported.</span></span> |
|<span data-ttu-id="9e449-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e449-115">Application</span></span>                            | <span data-ttu-id="9e449-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e449-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e449-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e449-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e449-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e449-118">Optional query parameters</span></span>
<span data-ttu-id="9e449-119">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e449-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e449-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e449-120">Request headers</span></span>
| <span data-ttu-id="9e449-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9e449-121">Name</span></span>      |<span data-ttu-id="9e449-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e449-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e449-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e449-123">Authorization</span></span>  | <span data-ttu-id="9e449-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e449-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e449-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e449-126">Request body</span></span>
<span data-ttu-id="9e449-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e449-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e449-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e449-128">Response</span></span>
<span data-ttu-id="9e449-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e449-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e449-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e449-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e449-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e449-131">Request</span></span>
<span data-ttu-id="9e449-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e449-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e449-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e449-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="c"></a>[<span data-ttu-id="9e449-134">C#</span><span class="sxs-lookup"><span data-stu-id="9e449-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e449-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e449-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e449-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e449-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e449-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e449-137">Response</span></span>
<span data-ttu-id="9e449-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e449-138">The following is an example of the response.</span></span> <span data-ttu-id="9e449-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9e449-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e449-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e449-140">All of the properties will be returned from an actual call.</span></span>
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
