---
title: Lista secureScores
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: f5466e24d6b523809a72f712666063808987e530
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034735"
---
# <a name="list-securescores"></a><span data-ttu-id="f3b97-104">Lista secureScores</span><span class="sxs-lookup"><span data-stu-id="f3b97-104">List secureScores</span></span>

 > <span data-ttu-id="f3b97-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3b97-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3b97-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3b97-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3b97-107">Recupere as propriedades e relacionamentos de um objeto [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="f3b97-107">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3b97-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f3b97-108">Permissions</span></span>

<span data-ttu-id="f3b97-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3b97-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3b97-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3b97-111">Permission type</span></span>      | <span data-ttu-id="f3b97-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3b97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3b97-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3b97-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f3b97-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="f3b97-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="f3b97-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3b97-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f3b97-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3b97-116">Not supported.</span></span>  |
|<span data-ttu-id="f3b97-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3b97-117">Application</span></span> | <span data-ttu-id="f3b97-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="f3b97-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3b97-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3b97-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="f3b97-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b97-120">Request headers</span></span>

| <span data-ttu-id="f3b97-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f3b97-121">Name</span></span>      |<span data-ttu-id="f3b97-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3b97-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3b97-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3b97-123">Authorization</span></span>  | <span data-ttu-id="f3b97-p104">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3b97-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3b97-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b97-126">Request body</span></span>

<span data-ttu-id="f3b97-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3b97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3b97-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3b97-128">Response</span></span>

<span data-ttu-id="f3b97-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b97-129">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3b97-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3b97-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3b97-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b97-131">Request</span></span>

<span data-ttu-id="f3b97-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3b97-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="f3b97-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3b97-133">Response</span></span>

<span data-ttu-id="f3b97-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b97-134">The following is an example of the response.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
