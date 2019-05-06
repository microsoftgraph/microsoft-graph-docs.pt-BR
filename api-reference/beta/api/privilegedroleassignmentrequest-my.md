---
title: 'privilegedRoleAssignmentRequest: My'
description: Obtenha as solicitações de atribuição de função privilegiada do solicitante.
localization_priority: Normal
ms.openlocfilehash: eb17e85e7ef4eb71892b2e1aeb84c5a8c22ac8ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593862"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="6888f-103">privilegedRoleAssignmentRequest: My</span><span class="sxs-lookup"><span data-stu-id="6888f-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6888f-104">Obtenha as solicitações de atribuição de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="6888f-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="6888f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6888f-105">Permissions</span></span>
<span data-ttu-id="6888f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6888f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6888f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6888f-108">Permission type</span></span>                        | <span data-ttu-id="6888f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6888f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6888f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6888f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6888f-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6888f-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6888f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6888f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6888f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6888f-113">Not supported.</span></span> |
|<span data-ttu-id="6888f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6888f-114">Application</span></span>                            | <span data-ttu-id="6888f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6888f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6888f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6888f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6888f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6888f-117">Optional query parameters</span></span>
<span data-ttu-id="6888f-118">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6888f-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6888f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6888f-119">Request headers</span></span>
| <span data-ttu-id="6888f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6888f-120">Name</span></span>      |<span data-ttu-id="6888f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6888f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6888f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6888f-122">Authorization</span></span>  | <span data-ttu-id="6888f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6888f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6888f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6888f-125">Request body</span></span>
<span data-ttu-id="6888f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6888f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6888f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6888f-127">Response</span></span>
<span data-ttu-id="6888f-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6888f-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6888f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6888f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6888f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6888f-130">Request</span></span>
<span data-ttu-id="6888f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6888f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="6888f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6888f-132">Response</span></span>
<span data-ttu-id="6888f-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6888f-133">The following is an example of the response.</span></span> <span data-ttu-id="6888f-134">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6888f-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6888f-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6888f-135">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6888f-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6888f-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6888f-137">Basic</span><span class="sxs-lookup"><span data-stu-id="6888f-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedroleassignmentrequest_my-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6888f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6888f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedroleassignmentrequest_my-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-my.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-my.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
