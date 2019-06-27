---
title: Listar secureScoreControlProfiles
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfiles.
localization_priority: Normal
ms.openlocfilehash: 220051afcb0d53b8e24482f8531a8442289357c5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269052"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="aeb44-103">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="aeb44-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeb44-104">Recupera uma lista de objetos [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) para um locatário.</span><span class="sxs-lookup"><span data-stu-id="aeb44-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeb44-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aeb44-105">Permissions</span></span>

<span data-ttu-id="aeb44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeb44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeb44-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aeb44-108">Permission type</span></span>      | <span data-ttu-id="aeb44-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aeb44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aeb44-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aeb44-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="aeb44-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="aeb44-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="aeb44-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aeb44-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aeb44-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aeb44-113">Not supported.</span></span>  |
|<span data-ttu-id="aeb44-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aeb44-114">Application</span></span> | <span data-ttu-id="aeb44-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="aeb44-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aeb44-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aeb44-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="aeb44-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb44-117">Request headers</span></span>

| <span data-ttu-id="aeb44-118">Nome</span><span class="sxs-lookup"><span data-stu-id="aeb44-118">Name</span></span>      |<span data-ttu-id="aeb44-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeb44-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aeb44-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aeb44-120">Authorization</span></span>  | <span data-ttu-id="aeb44-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="aeb44-121">Bearer {code}.</span></span> <span data-ttu-id="aeb44-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aeb44-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeb44-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb44-123">Request body</span></span>

<span data-ttu-id="aeb44-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aeb44-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeb44-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeb44-125">Response</span></span>

<span data-ttu-id="aeb44-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScoreControlProfile** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aeb44-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeb44-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aeb44-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="aeb44-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aeb44-128">Request</span></span>

<span data-ttu-id="aeb44-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aeb44-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="aeb44-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeb44-130">Response</span></span>

<span data-ttu-id="aeb44-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aeb44-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
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
            "deprecated": true,
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": 1020.13,
            "rank": 100,
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="aeb44-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="aeb44-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aeb44-133">C#</span><span class="sxs-lookup"><span data-stu-id="aeb44-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aeb44-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="aeb44-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aeb44-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="aeb44-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
