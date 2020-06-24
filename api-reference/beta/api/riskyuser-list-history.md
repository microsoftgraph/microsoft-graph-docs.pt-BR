---
title: Listar histórico de riskyUser
description: Recuperar o histórico de riscos
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 581de42d3034a31a2ef3ac347c71d815b285ad88
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863324"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="149ec-103">Listar histórico de riskyUser</span><span class="sxs-lookup"><span data-stu-id="149ec-103">List history of riskyUser</span></span>

<span data-ttu-id="149ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="149ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="149ec-105">Obter o histórico de riscos de um recurso [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="149ec-105">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="149ec-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="149ec-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="149ec-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="149ec-107">Permissions</span></span>
<span data-ttu-id="149ec-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="149ec-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="149ec-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="149ec-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="149ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="149ec-110">Permission type</span></span>      | <span data-ttu-id="149ec-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="149ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="149ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="149ec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="149ec-113">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="149ec-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="149ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="149ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="149ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="149ec-115">Not supported.</span></span>    |
|<span data-ttu-id="149ec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="149ec-116">Application</span></span> | <span data-ttu-id="149ec-117">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="149ec-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="149ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="149ec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
GET /identityProtection/riskyUsers/{id}/history/
```


## <a name="request-headers"></a><span data-ttu-id="149ec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="149ec-119">Request headers</span></span>
| <span data-ttu-id="149ec-120">Nome</span><span class="sxs-lookup"><span data-stu-id="149ec-120">Name</span></span>      |<span data-ttu-id="149ec-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="149ec-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="149ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="149ec-122">Authorization</span></span>  | <span data-ttu-id="149ec-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="149ec-123">Bearer {token}.</span></span> <span data-ttu-id="149ec-124">Required.</span><span class="sxs-lookup"><span data-stu-id="149ec-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="149ec-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="149ec-125">Request body</span></span>
<span data-ttu-id="149ec-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="149ec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="149ec-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="149ec-127">Response</span></span>

<span data-ttu-id="149ec-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="149ec-128">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="149ec-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="149ec-129">Examples</span></span>
### <a name="example-1-list-history-of-a-specific-user"></a><span data-ttu-id="149ec-130">Exemplo 1: listar histórico de um usuário específico</span><span class="sxs-lookup"><span data-stu-id="149ec-130">Example 1: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="149ec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="149ec-131">Request</span></span>
<span data-ttu-id="149ec-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="149ec-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="149ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="149ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="149ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="149ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="149ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="149ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="149ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="149ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="149ec-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="149ec-137">Response</span></span>
<span data-ttu-id="149ec-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="149ec-138">Here is an example of the response.</span></span>
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
### <a name="example-2-list-history-of-a-specific-user"></a><span data-ttu-id="149ec-139">Exemplo 2: listar histórico de um usuário específico</span><span class="sxs-lookup"><span data-stu-id="149ec-139">Example 2: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="149ec-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="149ec-140">Request</span></span>
<span data-ttu-id="149ec-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="149ec-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="149ec-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="149ec-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="149ec-143">C#</span><span class="sxs-lookup"><span data-stu-id="149ec-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="149ec-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="149ec-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="149ec-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="149ec-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="149ec-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="149ec-146">Response</span></span>
<span data-ttu-id="149ec-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="149ec-147">Here is an example of the response.</span></span>
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

