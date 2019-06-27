---
title: Listar histórico de riskyUser
description: Recuperar o histórico de riscos
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e33303b64cf9ff8b83e86a080e0c39ccf7c5f83c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267064"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="c16d9-103">Listar histórico de riskyUser</span><span class="sxs-lookup"><span data-stu-id="c16d9-103">List history of riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c16d9-104">Obter o histórico de riscos de um recurso [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="c16d9-104">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="c16d9-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c16d9-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="c16d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c16d9-106">Permissions</span></span>
<span data-ttu-id="c16d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c16d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c16d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c16d9-109">Permission type</span></span>      | <span data-ttu-id="c16d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c16d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c16d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c16d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c16d9-112">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c16d9-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="c16d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c16d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c16d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c16d9-114">Not supported.</span></span>    |
|<span data-ttu-id="c16d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c16d9-115">Application</span></span> | <span data-ttu-id="c16d9-116">Identityriskuser. Read. All, IdentityRiskUser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c16d9-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c16d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c16d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="c16d9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c16d9-118">Request headers</span></span>
| <span data-ttu-id="c16d9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c16d9-119">Name</span></span>      |<span data-ttu-id="c16d9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c16d9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c16d9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c16d9-121">Authorization</span></span>  | <span data-ttu-id="c16d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c16d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c16d9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c16d9-124">Request body</span></span>
<span data-ttu-id="c16d9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c16d9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c16d9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c16d9-126">Response</span></span>

<span data-ttu-id="c16d9-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c16d9-127">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c16d9-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c16d9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c16d9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c16d9-129">Request</span></span>
<span data-ttu-id="c16d9-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c16d9-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
##### <a name="response"></a><span data-ttu-id="c16d9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c16d9-131">Response</span></span>
<span data-ttu-id="c16d9-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c16d9-132">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c16d9-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c16d9-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c16d9-134">C#</span><span class="sxs-lookup"><span data-stu-id="c16d9-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_userriskhitsory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c16d9-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c16d9-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_userriskhitsory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c16d9-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c16d9-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_userriskhitsory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user risk history",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyuser-list-history.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyuser-list-history.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyuser-list-history.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

