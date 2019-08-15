---
title: Listar privilegedRoleAssignmentRequests
description: 'Recupere uma coleção de privilegedRoleAssignmentRequest. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b014615714ea0535a4683013445deac6684dcfda
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412632"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="0bdb0-103">Listar privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="0bdb0-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bdb0-104">Recupere uma coleção de [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0bdb0-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="0bdb0-105">**Observação:** Esse solicitante deve ter pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bdb0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0bdb0-106">Permissions</span></span>
<span data-ttu-id="0bdb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bdb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bdb0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bdb0-109">Permission type</span></span>                        | <span data-ttu-id="0bdb0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bdb0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bdb0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bdb0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0bdb0-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="0bdb0-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bdb0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bdb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bdb0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-114">Not supported.</span></span> |
|<span data-ttu-id="0bdb0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bdb0-115">Application</span></span>                            | <span data-ttu-id="0bdb0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bdb0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bdb0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0bdb0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0bdb0-118">Optional query parameters</span></span>
<span data-ttu-id="0bdb0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bdb0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bdb0-120">Request headers</span></span>
| <span data-ttu-id="0bdb0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0bdb0-121">Name</span></span>      |<span data-ttu-id="0bdb0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bdb0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0bdb0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bdb0-123">Authorization</span></span>  | <span data-ttu-id="0bdb0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bdb0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bdb0-126">Request body</span></span>
<span data-ttu-id="0bdb0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bdb0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bdb0-128">Response</span></span>
<span data-ttu-id="0bdb0-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bdb0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bdb0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bdb0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bdb0-131">Request</span></span>
<span data-ttu-id="0bdb0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0bdb0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bdb0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0bdb0-134">C#</span><span class="sxs-lookup"><span data-stu-id="0bdb0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bdb0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bdb0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0bdb0-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0bdb0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0bdb0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bdb0-137">Response</span></span>
<span data-ttu-id="0bdb0-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-138">The following is an example of the response.</span></span> <span data-ttu-id="0bdb0-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0bdb0-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bdb0-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "@odata.context":"https://https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
  "value":[
    {
      "schedule":{
        "type":"activation","startDateTime":"2018-02-07T22:55:00Z","endDateTime":null,"duration" : null
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
