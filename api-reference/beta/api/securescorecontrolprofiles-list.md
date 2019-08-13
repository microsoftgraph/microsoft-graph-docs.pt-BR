---
title: Listar secureScoreControlProfiles
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfiles.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: bffb18a0781150b347c0d8e2e1bc2d9be359cfd9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364240"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="dc509-103">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="dc509-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc509-104">Recupera uma lista de objetos [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) para um locatário.</span><span class="sxs-lookup"><span data-stu-id="dc509-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc509-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc509-105">Permissions</span></span>

<span data-ttu-id="dc509-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc509-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc509-108">Permission type</span></span>      | <span data-ttu-id="dc509-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc509-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc509-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc509-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="dc509-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="dc509-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="dc509-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc509-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dc509-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc509-113">Not supported.</span></span>  |
|<span data-ttu-id="dc509-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc509-114">Application</span></span> | <span data-ttu-id="dc509-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="dc509-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc509-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc509-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="dc509-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc509-117">Request headers</span></span>

| <span data-ttu-id="dc509-118">Nome</span><span class="sxs-lookup"><span data-stu-id="dc509-118">Name</span></span>      |<span data-ttu-id="dc509-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc509-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc509-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc509-120">Authorization</span></span>  | <span data-ttu-id="dc509-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="dc509-121">Bearer {code}.</span></span> <span data-ttu-id="dc509-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc509-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc509-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc509-123">Request body</span></span>

<span data-ttu-id="dc509-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc509-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc509-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc509-125">Response</span></span>

<span data-ttu-id="dc509-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScoreControlProfile** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc509-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc509-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc509-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc509-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc509-128">Request</span></span>

<span data-ttu-id="dc509-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc509-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc509-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc509-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc509-131">C#</span><span class="sxs-lookup"><span data-stu-id="dc509-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc509-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc509-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc509-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dc509-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc509-134">Java</span><span class="sxs-lookup"><span data-stu-id="dc509-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc509-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc509-135">Response</span></span>

<span data-ttu-id="dc509-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc509-136">The following is an example of the response.</span></span>
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
