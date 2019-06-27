---
title: Obter o item de histórico de riskyUser
description: Obter um item de histórico de um objeto riskyUser.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37ab3b0598ce54bec38fbd3feb719b1b0b2047bf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264999"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="c3f5d-103">Obter riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="c3f5d-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3f5d-104">Obter um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) de um [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="c3f5d-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="c3f5d-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3f5d-106">Permissions</span></span>
<span data-ttu-id="c3f5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3f5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3f5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3f5d-109">Permission type</span></span>      | <span data-ttu-id="c3f5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3f5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3f5d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3f5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3f5d-112">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3f5d-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3f5d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3f5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3f5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-114">Not supported.</span></span>    |
|<span data-ttu-id="c3f5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3f5d-115">Application</span></span> | <span data-ttu-id="c3f5d-116">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3f5d-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3f5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f5d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="c3f5d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f5d-118">Request headers</span></span>
| <span data-ttu-id="c3f5d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c3f5d-119">Name</span></span>      |<span data-ttu-id="c3f5d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f5d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3f5d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3f5d-121">Authorization</span></span>  | <span data-ttu-id="c3f5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3f5d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f5d-124">Request body</span></span>
<span data-ttu-id="c3f5d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3f5d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f5d-126">Response</span></span>

<span data-ttu-id="c3f5d-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3f5d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3f5d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3f5d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f5d-129">Request</span></span>
<span data-ttu-id="c3f5d-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
##### <a name="response"></a><span data-ttu-id="c3f5d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f5d-131">Response</span></span>
<span data-ttu-id="c3f5d-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f5d-132">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c3f5d-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c3f5d-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c3f5d-134">C#</span><span class="sxs-lookup"><span data-stu-id="c3f5d-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3f5d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3f5d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c3f5d-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3f5d-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

