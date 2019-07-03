---
title: Obter o item de histórico de riskyUser
description: Obter um item de histórico de um objeto riskyUser.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba51f6524630b6dfefc4e6106a626c7a40437963
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447701"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="6644d-103">Obter riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="6644d-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6644d-104">Obter um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) de um [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="6644d-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="6644d-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="6644d-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="6644d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6644d-106">Permissions</span></span>
<span data-ttu-id="6644d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6644d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6644d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6644d-109">Permission type</span></span>      | <span data-ttu-id="6644d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6644d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6644d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6644d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6644d-112">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6644d-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="6644d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6644d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6644d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6644d-114">Not supported.</span></span>    |
|<span data-ttu-id="6644d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6644d-115">Application</span></span> | <span data-ttu-id="6644d-116">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6644d-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6644d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6644d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="6644d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6644d-118">Request headers</span></span>
| <span data-ttu-id="6644d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6644d-119">Name</span></span>      |<span data-ttu-id="6644d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6644d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6644d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6644d-121">Authorization</span></span>  | <span data-ttu-id="6644d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6644d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6644d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6644d-124">Request body</span></span>
<span data-ttu-id="6644d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6644d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6644d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6644d-126">Response</span></span>

<span data-ttu-id="6644d-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6644d-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6644d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6644d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6644d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6644d-129">Request</span></span>
<span data-ttu-id="6644d-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6644d-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6644d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6644d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6644d-132">C#</span><span class="sxs-lookup"><span data-stu-id="6644d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6644d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6644d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6644d-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6644d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6644d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6644d-135">Response</span></span>
<span data-ttu-id="6644d-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6644d-136">Here is an example of the response.</span></span>
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

