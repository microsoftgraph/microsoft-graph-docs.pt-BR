---
title: Listar secureScoreControlProfiles
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfiles.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b0b2fea39c8fb4a9bdcb8bc3d16a3273ac8eb8ef
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330183"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="6016f-103">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6016f-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="6016f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6016f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6016f-105">Recupere as propriedades e os relacionamentos de um objeto [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6016f-105">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6016f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6016f-106">Permissions</span></span>

<span data-ttu-id="6016f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6016f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6016f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6016f-109">Permission type</span></span>      | <span data-ttu-id="6016f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6016f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6016f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6016f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6016f-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6016f-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="6016f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6016f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6016f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6016f-114">Not supported.</span></span>  |
|<span data-ttu-id="6016f-115">Application</span><span class="sxs-lookup"><span data-stu-id="6016f-115">Application</span></span> | <span data-ttu-id="6016f-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6016f-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6016f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6016f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6016f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6016f-118">Optional query parameters</span></span>

<span data-ttu-id="6016f-119">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="6016f-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="6016f-120">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="6016f-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="6016f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6016f-121">Request headers</span></span>

| <span data-ttu-id="6016f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6016f-122">Name</span></span>      |<span data-ttu-id="6016f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6016f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6016f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6016f-124">Authorization</span></span>  | <span data-ttu-id="6016f-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="6016f-125">Bearer {code}.</span></span> <span data-ttu-id="6016f-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6016f-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6016f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6016f-127">Request body</span></span>

<span data-ttu-id="6016f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6016f-128">Do not supply a request body for this method.</span></span> <span data-ttu-id="6016f-129">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="6016f-129">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="6016f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6016f-130">Response</span></span>

<span data-ttu-id="6016f-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos **secureScoreControlProfiles** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6016f-131">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6016f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6016f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6016f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6016f-133">Request</span></span>

<span data-ttu-id="6016f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6016f-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6016f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6016f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```
# <a name="c"></a>[<span data-ttu-id="6016f-136">C#</span><span class="sxs-lookup"><span data-stu-id="6016f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofiles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6016f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6016f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofiles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6016f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6016f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofiles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6016f-139">Java</span><span class="sxs-lookup"><span data-stu-id="6016f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofiles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6016f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6016f-140">Response</span></span>

<span data-ttu-id="6016f-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6016f-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "value": [
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
              "name":  "A.8.2.1",
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

