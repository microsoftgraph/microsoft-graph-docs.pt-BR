---
title: Obter o item de histórico de riskyUser
description: Obter um item de histórico de um objeto riskyUser.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b185444057349700978786f235249f6222ebfbb9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960918"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="533e5-103">Obter riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="533e5-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="533e5-104">Obter um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) de um [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="533e5-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="533e5-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="533e5-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="533e5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="533e5-106">Permissions</span></span>
<span data-ttu-id="533e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="533e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="533e5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="533e5-109">Permission type</span></span>      | <span data-ttu-id="533e5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="533e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="533e5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="533e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="533e5-112">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="533e5-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="533e5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="533e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="533e5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="533e5-114">Not supported.</span></span>    |
|<span data-ttu-id="533e5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="533e5-115">Application</span></span> | <span data-ttu-id="533e5-116">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="533e5-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="533e5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="533e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="533e5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="533e5-118">Request headers</span></span>
| <span data-ttu-id="533e5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="533e5-119">Name</span></span>      |<span data-ttu-id="533e5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="533e5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="533e5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="533e5-121">Authorization</span></span>  | <span data-ttu-id="533e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="533e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="533e5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="533e5-124">Request body</span></span>
<span data-ttu-id="533e5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="533e5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="533e5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="533e5-126">Response</span></span>

<span data-ttu-id="533e5-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="533e5-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="533e5-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="533e5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="533e5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="533e5-129">Request</span></span>
<span data-ttu-id="533e5-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="533e5-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
##### <a name="response"></a><span data-ttu-id="533e5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="533e5-131">Response</span></span>
<span data-ttu-id="533e5-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="533e5-132">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="533e5-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="533e5-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="533e5-134">C#</span><span class="sxs-lookup"><span data-stu-id="533e5-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="533e5-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="533e5-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUserHistoryItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

