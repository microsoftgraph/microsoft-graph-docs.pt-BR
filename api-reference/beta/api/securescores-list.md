---
title: Lista secureScores
description: Recupere as propriedades e relacionamentos de um objeto secureScores.
localization_priority: Normal
ms.openlocfilehash: e574c3e52eb60f29dac89e2795b04666c7a1f02b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521478"
---
# <a name="list-securescores"></a><span data-ttu-id="4053b-103">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="4053b-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4053b-104">Recupere as propriedades e relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="4053b-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4053b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4053b-105">Permissions</span></span>

<span data-ttu-id="4053b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4053b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4053b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4053b-108">Permission type</span></span>      | <span data-ttu-id="4053b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4053b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4053b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4053b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4053b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="4053b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="4053b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4053b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4053b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4053b-113">Not supported.</span></span>  |
|<span data-ttu-id="4053b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4053b-114">Application</span></span> | <span data-ttu-id="4053b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="4053b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4053b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4053b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="4053b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4053b-117">Request headers</span></span>

| <span data-ttu-id="4053b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4053b-118">Name</span></span>      |<span data-ttu-id="4053b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4053b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4053b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4053b-120">Authorization</span></span>  | <span data-ttu-id="4053b-p102">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4053b-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4053b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4053b-123">Request body</span></span>

<span data-ttu-id="4053b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4053b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4053b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4053b-125">Response</span></span>

<span data-ttu-id="4053b-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4053b-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4053b-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4053b-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="4053b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4053b-128">Request</span></span>

<span data-ttu-id="4053b-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4053b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="4053b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4053b-130">Response</span></span>

<span data-ttu-id="4053b-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4053b-131">The following is an example of the response.</span></span>
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
