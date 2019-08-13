---
title: Listar secureScores
description: Recupere as propriedades e os relacionamentos de um objeto secureScores.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 76642b168d4d1361ce50a9d938696840df1c7fea
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364177"
---
# <a name="list-securescores"></a><span data-ttu-id="7811a-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="7811a-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7811a-104">Recupere as propriedades e os relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="7811a-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7811a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7811a-105">Permissions</span></span>

<span data-ttu-id="7811a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7811a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7811a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7811a-108">Permission type</span></span>      | <span data-ttu-id="7811a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7811a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7811a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7811a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7811a-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="7811a-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="7811a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7811a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7811a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7811a-113">Not supported.</span></span>  |
|<span data-ttu-id="7811a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7811a-114">Application</span></span> | <span data-ttu-id="7811a-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="7811a-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7811a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7811a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="7811a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7811a-117">Request headers</span></span>

| <span data-ttu-id="7811a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7811a-118">Name</span></span>      |<span data-ttu-id="7811a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7811a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7811a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7811a-120">Authorization</span></span>  | <span data-ttu-id="7811a-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="7811a-121">Bearer {code}.</span></span> <span data-ttu-id="7811a-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7811a-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7811a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7811a-123">Request body</span></span>

<span data-ttu-id="7811a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7811a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7811a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7811a-125">Response</span></span>

<span data-ttu-id="7811a-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7811a-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7811a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7811a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="7811a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7811a-128">Request</span></span>

<span data-ttu-id="7811a-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7811a-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7811a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7811a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7811a-131">C#</span><span class="sxs-lookup"><span data-stu-id="7811a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7811a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7811a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7811a-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7811a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7811a-134">Java</span><span class="sxs-lookup"><span data-stu-id="7811a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescores-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7811a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7811a-135">Response</span></span>

<span data-ttu-id="7811a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7811a-136">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
