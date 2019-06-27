---
title: Listar secureScores
description: Recupere as propriedades e os relacionamentos de um objeto secureScores.
localization_priority: Normal
ms.openlocfilehash: 36afa8bdf8d588d8d8b030d30a4e8cf41ba08855
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263893"
---
# <a name="list-securescores"></a><span data-ttu-id="a69e5-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="a69e5-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a69e5-104">Recupere as propriedades e os relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="a69e5-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a69e5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a69e5-105">Permissions</span></span>

<span data-ttu-id="a69e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a69e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69e5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a69e5-108">Permission type</span></span>      | <span data-ttu-id="a69e5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a69e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a69e5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a69e5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a69e5-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="a69e5-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="a69e5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a69e5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a69e5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a69e5-113">Not supported.</span></span>  |
|<span data-ttu-id="a69e5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a69e5-114">Application</span></span> | <span data-ttu-id="a69e5-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="a69e5-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a69e5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a69e5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="a69e5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a69e5-117">Request headers</span></span>

| <span data-ttu-id="a69e5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a69e5-118">Name</span></span>      |<span data-ttu-id="a69e5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a69e5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a69e5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a69e5-120">Authorization</span></span>  | <span data-ttu-id="a69e5-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="a69e5-121">Bearer {code}.</span></span> <span data-ttu-id="a69e5-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a69e5-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a69e5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a69e5-123">Request body</span></span>

<span data-ttu-id="a69e5-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a69e5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a69e5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69e5-125">Response</span></span>

<span data-ttu-id="a69e5-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a69e5-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69e5-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a69e5-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="a69e5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a69e5-128">Request</span></span>

<span data-ttu-id="a69e5-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a69e5-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="a69e5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69e5-130">Response</span></span>

<span data-ttu-id="a69e5-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a69e5-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection":true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 1,
            "createdDateTime": "createdDateTime.value",
            "currentScore": 1,
            "enabledServices": "enabledServices.value",
            "licensedUserCount": 1,
            "maxScore": 1,
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a69e5-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="a69e5-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a69e5-133">C#</span><span class="sxs-lookup"><span data-stu-id="a69e5-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescores_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a69e5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a69e5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescores_list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a69e5-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a69e5-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/securescores_list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
