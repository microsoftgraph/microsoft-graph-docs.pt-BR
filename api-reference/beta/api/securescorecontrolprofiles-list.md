---
title: Lista secureScoreControlProfiles
description: Recupere as propriedades e relacionamentos de um objeto secureScoreControlProfiles.
localization_priority: Normal
ms.openlocfilehash: 6627111633f54eb7bc2584af826b69fd5bd6cf49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508052"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="60f79-103">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="60f79-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60f79-104">Recupere as propriedades e relacionamentos de um objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) .</span><span class="sxs-lookup"><span data-stu-id="60f79-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60f79-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="60f79-105">Permissions</span></span>

<span data-ttu-id="60f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60f79-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60f79-108">Permission type</span></span>      | <span data-ttu-id="60f79-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60f79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60f79-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60f79-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="60f79-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="60f79-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="60f79-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60f79-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="60f79-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60f79-113">Not supported.</span></span>  |
|<span data-ttu-id="60f79-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60f79-114">Application</span></span> | <span data-ttu-id="60f79-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="60f79-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60f79-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60f79-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="60f79-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60f79-117">Request headers</span></span>

| <span data-ttu-id="60f79-118">Nome</span><span class="sxs-lookup"><span data-stu-id="60f79-118">Name</span></span>      |<span data-ttu-id="60f79-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="60f79-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60f79-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="60f79-120">Authorization</span></span>  | <span data-ttu-id="60f79-p102">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60f79-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60f79-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60f79-123">Request body</span></span>

<span data-ttu-id="60f79-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60f79-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60f79-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f79-125">Response</span></span>

<span data-ttu-id="60f79-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **secureScoreControlProfiles** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60f79-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60f79-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60f79-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="60f79-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60f79-128">Request</span></span>

<span data-ttu-id="60f79-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60f79-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="60f79-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f79-130">Response</span></span>

<span data-ttu-id="60f79-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60f79-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "actionType": "actionType.value",
            "actionUrl": "actionUrl.value",
            "controlCategory": "controlCategory.value",
            "title": "title.value",
            "deprecated": "deprecated.value",
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": "maxScore.value",
            "rank": "rank.value",
            "remediation": "remediation.value",
            "remediationImpact": "remediationImpact.value",
            "service": "service.value",
            "threats": [
                "threats.value"
            ],
            "tier": "tier.value",
            "userImpact": "userImpact.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "controlStateUpdates": [
                {
                    "assignedTo": "assignedTo.value",
                    "comment": "comment.value",
                    "state": "state.value",
                    "updatedBy": "updatedBy.value",
                    "updatedDateTime": "updatedDateTime.value"
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
         }
     ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
