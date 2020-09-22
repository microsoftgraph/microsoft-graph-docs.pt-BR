---
title: Listar secureScoreControlProfiles
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfiles.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7e570c6fdbd23920393d5530fdf7a0104c19b385
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067542"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="e8acb-103">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="e8acb-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="e8acb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8acb-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8acb-105">Recupera uma lista de objetos [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) para um locatário.</span><span class="sxs-lookup"><span data-stu-id="e8acb-105">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8acb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8acb-106">Permissions</span></span>

<span data-ttu-id="e8acb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8acb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8acb-109">Permission type</span></span>      | <span data-ttu-id="e8acb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8acb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8acb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8acb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8acb-112">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="e8acb-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e8acb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8acb-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8acb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8acb-114">Not supported.</span></span>  |
|<span data-ttu-id="e8acb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8acb-115">Application</span></span> | <span data-ttu-id="e8acb-116">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="e8acb-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8acb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8acb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e8acb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8acb-118">Request headers</span></span>

| <span data-ttu-id="e8acb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e8acb-119">Name</span></span>      |<span data-ttu-id="e8acb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8acb-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8acb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8acb-121">Authorization</span></span>  | <span data-ttu-id="e8acb-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="e8acb-122">Bearer {code}.</span></span> <span data-ttu-id="e8acb-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8acb-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8acb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8acb-124">Request body</span></span>

<span data-ttu-id="e8acb-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8acb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8acb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8acb-126">Response</span></span>

<span data-ttu-id="e8acb-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos **secureScoreControlProfile** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8acb-127">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8acb-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8acb-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8acb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8acb-129">Request</span></span>

<span data-ttu-id="e8acb-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8acb-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8acb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8acb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```
# <a name="c"></a>[<span data-ttu-id="e8acb-132">C#</span><span class="sxs-lookup"><span data-stu-id="e8acb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8acb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8acb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8acb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8acb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8acb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8acb-135">Response</span></span>

<span data-ttu-id="e8acb-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8acb-136">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


