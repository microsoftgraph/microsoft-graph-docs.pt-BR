---
title: Obter o item de histórico de riskyUser
description: Obter um item de histórico de um objeto riskyUser.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db2743525ecb291f4d07afe6ea6ce379b938bfe4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863520"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="1939e-103">Obter riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="1939e-103">Get riskyUserHistoryItem</span></span>

<span data-ttu-id="1939e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1939e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1939e-105">Obter um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) de um [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="1939e-105">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="1939e-106">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="1939e-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1939e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1939e-107">Permissions</span></span>
<span data-ttu-id="1939e-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1939e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1939e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1939e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1939e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1939e-110">Permission type</span></span>      | <span data-ttu-id="1939e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1939e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1939e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1939e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1939e-113">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1939e-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="1939e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1939e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1939e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1939e-115">Not supported.</span></span>    |
|<span data-ttu-id="1939e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1939e-116">Application</span></span> | <span data-ttu-id="1939e-117">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1939e-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1939e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1939e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
GET /identityProtection/riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="1939e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1939e-119">Request headers</span></span>
| <span data-ttu-id="1939e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1939e-120">Name</span></span>      |<span data-ttu-id="1939e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1939e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1939e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1939e-122">Authorization</span></span>  | <span data-ttu-id="1939e-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="1939e-123">Bearer {token}.</span></span> <span data-ttu-id="1939e-124">Required.</span><span class="sxs-lookup"><span data-stu-id="1939e-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1939e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1939e-125">Request body</span></span>
<span data-ttu-id="1939e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1939e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1939e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1939e-127">Response</span></span>

<span data-ttu-id="1939e-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1939e-128">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1939e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1939e-129">Examples</span></span>
### <a name="example-1-get-history-of-a-risky-user"></a><span data-ttu-id="1939e-130">Exemplo 1: obter o histórico de um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="1939e-130">Example 1: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="1939e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1939e-131">Request</span></span>
<span data-ttu-id="1939e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1939e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1939e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1939e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="1939e-134">C#</span><span class="sxs-lookup"><span data-stu-id="1939e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1939e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1939e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1939e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1939e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1939e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1939e-137">Response</span></span>
<span data-ttu-id="1939e-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1939e-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```

### <a name="example-2-get-history-of-a-risky-user"></a><span data-ttu-id="1939e-139">Exemplo 2: obter o histórico de um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="1939e-139">Example 2: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="1939e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1939e-140">Request</span></span>
<span data-ttu-id="1939e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1939e-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1939e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1939e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="1939e-143">C#</span><span class="sxs-lookup"><span data-stu-id="1939e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1939e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1939e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1939e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1939e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1939e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1939e-146">Response</span></span>
<span data-ttu-id="1939e-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1939e-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUserHistoryItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

