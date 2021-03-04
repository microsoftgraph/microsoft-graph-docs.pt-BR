---
title: Obter item de histórico de riskyUser
description: Obter um item de histórico de um objeto riskyUser.
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 78eb02bb7667625ef71aba1a5ad5f3d2e3fc252f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443563"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="1b5bb-103">Obter riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="1b5bb-103">Get riskyUserHistoryItem</span></span>

<span data-ttu-id="1b5bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b5bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b5bb-105">Obter um [objeto riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) de [um riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="1b5bb-105">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="1b5bb-106">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b5bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b5bb-107">Permissions</span></span>
<span data-ttu-id="1b5bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b5bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b5bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b5bb-110">Permission type</span></span>      | <span data-ttu-id="1b5bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b5bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b5bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5bb-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5bb-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b5bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b5bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-115">Not supported.</span></span>    |
|<span data-ttu-id="1b5bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b5bb-116">Application</span></span> | <span data-ttu-id="1b5bb-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5bb-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b5bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
GET /identityProtection/riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="1b5bb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5bb-119">Request headers</span></span>
| <span data-ttu-id="1b5bb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1b5bb-120">Name</span></span>      |<span data-ttu-id="1b5bb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b5bb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b5bb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b5bb-122">Authorization</span></span>  | <span data-ttu-id="1b5bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b5bb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5bb-125">Request body</span></span>
<span data-ttu-id="1b5bb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b5bb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5bb-127">Response</span></span>

<span data-ttu-id="1b5bb-128">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-128">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b5bb-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b5bb-129">Examples</span></span>
### <a name="example-1-get-history-of-a-risky-user"></a><span data-ttu-id="1b5bb-130">Exemplo 1: obter histórico de um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="1b5bb-130">Example 1: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="1b5bb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5bb-131">Request</span></span>
<span data-ttu-id="1b5bb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b5bb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5bb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="1b5bb-134">C#</span><span class="sxs-lookup"><span data-stu-id="1b5bb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b5bb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b5bb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b5bb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b5bb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b5bb-137">Java</span><span class="sxs-lookup"><span data-stu-id="1b5bb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-historyitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1b5bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5bb-138">Response</span></span>
<span data-ttu-id="1b5bb-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-139">Here is an example of the response.</span></span>
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

### <a name="example-2-get-history-of-a-risky-user"></a><span data-ttu-id="1b5bb-140">Exemplo 2: Obter histórico de um usuário arriscado</span><span class="sxs-lookup"><span data-stu-id="1b5bb-140">Example 2: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="1b5bb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5bb-141">Request</span></span>
<span data-ttu-id="1b5bb-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b5bb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5bb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="1b5bb-144">C#</span><span class="sxs-lookup"><span data-stu-id="1b5bb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b5bb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b5bb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b5bb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b5bb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b5bb-147">Java</span><span class="sxs-lookup"><span data-stu-id="1b5bb-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-historyitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1b5bb-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5bb-148">Response</span></span>
<span data-ttu-id="1b5bb-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b5bb-149">Here is an example of the response.</span></span>
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



