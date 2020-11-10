---
title: Listar histórico de riskyUser
description: Recuperar o histórico de riscos
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0f19ee45387996436d47e92f90c98eddd5b9bbad
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977644"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="a2bb0-103">Listar histórico de riskyUser</span><span class="sxs-lookup"><span data-stu-id="a2bb0-103">List history of riskyUser</span></span>

<span data-ttu-id="a2bb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2bb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2bb0-105">Obter o histórico de riscos de um recurso [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="a2bb0-105">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="a2bb0-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2bb0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2bb0-107">Permissions</span></span>
<span data-ttu-id="a2bb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2bb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2bb0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2bb0-110">Permission type</span></span>      | <span data-ttu-id="a2bb0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2bb0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2bb0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2bb0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2bb0-113">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a2bb0-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2bb0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2bb0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2bb0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-115">Not supported.</span></span>    |
|<span data-ttu-id="a2bb0-116">Application</span><span class="sxs-lookup"><span data-stu-id="a2bb0-116">Application</span></span> | <span data-ttu-id="a2bb0-117">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a2bb0-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2bb0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2bb0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
GET /identityProtection/riskyUsers/{id}/history/
```


## <a name="request-headers"></a><span data-ttu-id="a2bb0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bb0-119">Request headers</span></span>
| <span data-ttu-id="a2bb0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a2bb0-120">Name</span></span>      |<span data-ttu-id="a2bb0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2bb0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2bb0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2bb0-122">Authorization</span></span>  | <span data-ttu-id="a2bb0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2bb0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bb0-125">Request body</span></span>
<span data-ttu-id="a2bb0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2bb0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bb0-127">Response</span></span>

<span data-ttu-id="a2bb0-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-128">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2bb0-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a2bb0-129">Examples</span></span>
### <a name="example-1-list-history-of-a-specific-user"></a><span data-ttu-id="a2bb0-130">Exemplo 1: listar histórico de um usuário específico</span><span class="sxs-lookup"><span data-stu-id="a2bb0-130">Example 1: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="a2bb0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bb0-131">Request</span></span>
<span data-ttu-id="a2bb0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2bb0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2bb0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="a2bb0-134">C#</span><span class="sxs-lookup"><span data-stu-id="a2bb0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2bb0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2bb0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2bb0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2bb0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2bb0-137">Java</span><span class="sxs-lookup"><span data-stu-id="a2bb0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userriskhitsory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a2bb0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bb0-138">Response</span></span>
<span data-ttu-id="a2bb0-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```
### <a name="example-2-list-history-of-a-specific-user"></a><span data-ttu-id="a2bb0-140">Exemplo 2: listar histórico de um usuário específico</span><span class="sxs-lookup"><span data-stu-id="a2bb0-140">Example 2: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="a2bb0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bb0-141">Request</span></span>
<span data-ttu-id="a2bb0-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2bb0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2bb0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="a2bb0-144">C#</span><span class="sxs-lookup"><span data-stu-id="a2bb0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2bb0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2bb0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2bb0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2bb0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2bb0-147">Java</span><span class="sxs-lookup"><span data-stu-id="a2bb0-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userriskhitsory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a2bb0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bb0-148">Response</span></span>
<span data-ttu-id="a2bb0-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bb0-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user risk history",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



