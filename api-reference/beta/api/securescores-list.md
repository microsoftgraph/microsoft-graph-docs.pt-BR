---
title: Listar secureScores
description: Recupere as propriedades e os relacionamentos de um objeto secureScores.
localization_priority: Normal
ms.openlocfilehash: e574c3e52eb60f29dac89e2795b04666c7a1f02b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545461"
---
# <a name="list-securescores"></a><span data-ttu-id="9ddb5-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="9ddb5-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ddb5-104">Recupere as propriedades e os relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="9ddb5-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ddb5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ddb5-105">Permissions</span></span>

<span data-ttu-id="9ddb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ddb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ddb5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ddb5-108">Permission type</span></span>      | <span data-ttu-id="9ddb5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ddb5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ddb5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ddb5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ddb5-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="9ddb5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ddb5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ddb5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-113">Not supported.</span></span>  |
|<span data-ttu-id="9ddb5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ddb5-114">Application</span></span> | <span data-ttu-id="9ddb5-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ddb5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ddb5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="9ddb5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ddb5-117">Request headers</span></span>

| <span data-ttu-id="9ddb5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9ddb5-118">Name</span></span>      |<span data-ttu-id="9ddb5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ddb5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ddb5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ddb5-120">Authorization</span></span>  | <span data-ttu-id="9ddb5-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-121">Bearer {code}.</span></span> <span data-ttu-id="9ddb5-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ddb5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ddb5-123">Request body</span></span>

<span data-ttu-id="9ddb5-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ddb5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ddb5-125">Response</span></span>

<span data-ttu-id="9ddb5-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ddb5-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ddb5-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ddb5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ddb5-128">Request</span></span>

<span data-ttu-id="9ddb5-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="9ddb5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ddb5-130">Response</span></span>

<span data-ttu-id="9ddb5-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ddb5-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScores"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "activeUserCount": "activeUserCount.value",
            "createdDateTime": "createdDateTime.value",
            "currentScore": "currentScore.value",
            "enabledServices": "enabledServices.value",
            "licensedUserCount": "licensedUserCount.value",
            "maxScore": "maxScore.value",
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
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
