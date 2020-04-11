---
title: Obter secureScoreControlProfile
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfile.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d5425dc8a2f908f0f7b4e3cf7120968bf4b51f7a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229595"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="9b696-103">Obter secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="9b696-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="9b696-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b696-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b696-105">Recupere as propriedades e os relacionamentos de um objeto [securescorecontrolprofile](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9b696-105">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b696-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b696-106">Permissions</span></span>

<span data-ttu-id="9b696-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b696-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b696-109">Permission type</span></span>      | <span data-ttu-id="9b696-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b696-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b696-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b696-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9b696-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b696-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="9b696-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b696-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9b696-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b696-114">Not supported.</span></span>  |
|<span data-ttu-id="9b696-115">Application</span><span class="sxs-lookup"><span data-stu-id="9b696-115">Application</span></span> | <span data-ttu-id="9b696-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b696-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b696-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b696-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9b696-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b696-118">Request headers</span></span>

| <span data-ttu-id="9b696-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9b696-119">Name</span></span>      |<span data-ttu-id="9b696-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b696-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b696-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b696-121">Authorization</span></span>  | <span data-ttu-id="9b696-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="9b696-122">Bearer {code}.</span></span> <span data-ttu-id="9b696-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b696-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b696-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b696-124">Request body</span></span>

<span data-ttu-id="9b696-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b696-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b696-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b696-126">Response</span></span>

<span data-ttu-id="9b696-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScoreControlProfile** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b696-127">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="9b696-128">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="9b696-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="9b696-129">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="9b696-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="9b696-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b696-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b696-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b696-131">Request</span></span>

<span data-ttu-id="9b696-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b696-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b696-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b696-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="9b696-134">C#</span><span class="sxs-lookup"><span data-stu-id="9b696-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b696-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b696-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b696-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b696-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b696-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b696-137">Response</span></span>

<span data-ttu-id="9b696-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b696-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "DLPEnabled",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Config",
  "actionUrl": "https://compliance.microsoft.com/#/policies",
  "controlCategory": "Data",
  "title": "Apply Data Loss Prevention policies", 
  "deprecated": false,
  "implementationCost": "Moderate",
  "lastModifiedDateTime": null,
  "maxScore": 20.0,
  "rank": 55,
  "remediation": "You can create and manage data loss prevention policies in the Policies page of the compliance portal.",
  "remediationImpact": "This change will have a moderate impact on your users.",
  "service": "IP",
  "threats": [
    "Data Exfiltration",
    "Data Spillage"
  ],
  "tier": "Advanced",
  "userImpact": "Moderate",
  "complianceInformation": [
    {
      "certificationName": "ISO 27001:2013",
      "certificationControls": [
        {
          "name": "A.8.2.1",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": null,
      "comment": null,
      "state": "Default",
      "updatedBy": null,
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "get secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
