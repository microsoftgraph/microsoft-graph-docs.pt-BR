---
title: Listar secureScores
description: Recupere as propriedades e os relacionamentos de um objeto secureScores.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f71862ecebb668da478cbf7ee56454f38a723399
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809933"
---
# <a name="list-securescores"></a><span data-ttu-id="e1600-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="e1600-103">List secureScores</span></span>

<span data-ttu-id="e1600-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1600-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1600-105">Recupere as propriedades e os relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="e1600-105">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1600-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1600-106">Permissions</span></span>

<span data-ttu-id="e1600-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1600-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1600-109">Permission type</span></span>      | <span data-ttu-id="e1600-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1600-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1600-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1600-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1600-112">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="e1600-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e1600-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1600-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1600-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1600-114">Not supported.</span></span>  |
|<span data-ttu-id="e1600-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1600-115">Application</span></span> | <span data-ttu-id="e1600-116">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="e1600-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1600-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1600-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="e1600-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1600-118">Request headers</span></span>

| <span data-ttu-id="e1600-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e1600-119">Name</span></span>      |<span data-ttu-id="e1600-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1600-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1600-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1600-121">Authorization</span></span>  | <span data-ttu-id="e1600-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="e1600-122">Bearer {code}.</span></span> <span data-ttu-id="e1600-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1600-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1600-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1600-124">Request body</span></span>

<span data-ttu-id="e1600-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1600-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1600-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1600-126">Response</span></span>

<span data-ttu-id="e1600-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1600-127">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1600-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1600-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1600-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1600-129">Request</span></span>

<span data-ttu-id="e1600-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1600-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1600-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1600-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="e1600-132">C#</span><span class="sxs-lookup"><span data-stu-id="e1600-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1600-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1600-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1600-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1600-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1600-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1600-135">Response</span></span>

<span data-ttu-id="e1600-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1600-136">The following is an example of the response.</span></span>
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
