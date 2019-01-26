---
title: Lista secureScores
description: Recupere as propriedades e relacionamentos de um objeto secureScores.
localization_priority: Normal
ms.openlocfilehash: 034a333dec6b96919ffd01a49ed05cb16ca19a48
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573400"
---
# <a name="list-securescores"></a><span data-ttu-id="286b4-103">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="286b4-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="286b4-104">Recupere as propriedades e relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="286b4-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="286b4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="286b4-105">Permissions</span></span>

<span data-ttu-id="286b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="286b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="286b4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="286b4-108">Permission type</span></span>      | <span data-ttu-id="286b4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="286b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="286b4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="286b4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="286b4-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="286b4-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="286b4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="286b4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="286b4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="286b4-113">Not supported.</span></span>  |
|<span data-ttu-id="286b4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="286b4-114">Application</span></span> | <span data-ttu-id="286b4-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="286b4-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="286b4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="286b4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="286b4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="286b4-117">Request headers</span></span>

| <span data-ttu-id="286b4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="286b4-118">Name</span></span>      |<span data-ttu-id="286b4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="286b4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="286b4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="286b4-120">Authorization</span></span>  | <span data-ttu-id="286b4-p102">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="286b4-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="286b4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="286b4-123">Request body</span></span>

<span data-ttu-id="286b4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="286b4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="286b4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="286b4-125">Response</span></span>

<span data-ttu-id="286b4-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="286b4-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="286b4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="286b4-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="286b4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="286b4-128">Request</span></span>

<span data-ttu-id="286b4-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="286b4-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="286b4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="286b4-130">Response</span></span>

<span data-ttu-id="286b4-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="286b4-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 12,
            "createdDate": "createdDateTime.value",
            "currentScore": 12.4566633444,
            "enabledServices": ["Skype"],
            "licensedUserCount": 12,
            "maxScore": 45.2324443,
            "id": "id.value",            
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                },
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                },
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                }
            ],
            "controlScores": [
                {
                    "@odata.type":"microsoft.graph.controlScores",
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
