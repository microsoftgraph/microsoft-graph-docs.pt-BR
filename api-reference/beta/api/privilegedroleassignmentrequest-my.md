---
title: 'privilegedRoleAssignmentRequest: meu'
description: Obtenha as solicitações de atribuição de função privilegiado do solicitante.
ms.openlocfilehash: a2e6ca655359594480e09127721813f73726e2e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039590"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="21e94-103">privilegedRoleAssignmentRequest: meu</span><span class="sxs-lookup"><span data-stu-id="21e94-103">privilegedRoleAssignmentRequest: my</span></span>

> <span data-ttu-id="21e94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21e94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21e94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21e94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21e94-106">Obtenha as solicitações de atribuição de função privilegiado do solicitante.</span><span class="sxs-lookup"><span data-stu-id="21e94-106">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="21e94-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="21e94-107">Permissions</span></span>
<span data-ttu-id="21e94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21e94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21e94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21e94-110">Permission type</span></span>                        | <span data-ttu-id="21e94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21e94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="21e94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21e94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21e94-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21e94-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21e94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21e94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21e94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21e94-115">Not supported.</span></span> |
|<span data-ttu-id="21e94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21e94-116">Application</span></span>                            | <span data-ttu-id="21e94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21e94-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21e94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21e94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="21e94-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21e94-119">Optional query parameters</span></span>
<span data-ttu-id="21e94-120">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21e94-120">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21e94-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21e94-121">Request headers</span></span>
| <span data-ttu-id="21e94-122">Nome</span><span class="sxs-lookup"><span data-stu-id="21e94-122">Name</span></span>      |<span data-ttu-id="21e94-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e94-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21e94-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="21e94-124">Authorization</span></span>  | <span data-ttu-id="21e94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21e94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21e94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21e94-127">Request body</span></span>
<span data-ttu-id="21e94-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21e94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21e94-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e94-129">Response</span></span>
<span data-ttu-id="21e94-130">Se tiver êxito, este método retornará `200 OK` objeto de coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21e94-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e94-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21e94-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21e94-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21e94-132">Request</span></span>
<span data-ttu-id="21e94-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21e94-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="21e94-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e94-134">Response</span></span>
<span data-ttu-id="21e94-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21e94-135">The following is an example of the response.</span></span> <span data-ttu-id="21e94-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="21e94-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="21e94-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21e94-137">All of the properties will be returned from an actual call.</span></span>
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
         "userId": "Self"，
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
        "userId": "Self"，
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
