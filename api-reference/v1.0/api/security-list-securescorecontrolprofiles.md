---
title: Listar secureScoreControlProfiles
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfiles.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: d7de3b6b446aa12447023d6b4f111fc2ac28b41e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629737"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="0c93a-103">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="0c93a-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="0c93a-104">Recupere as propriedades e os relacionamentos de um objeto [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0c93a-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c93a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c93a-105">Permissions</span></span>

<span data-ttu-id="0c93a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c93a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c93a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c93a-108">Permission type</span></span>      | <span data-ttu-id="0c93a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c93a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c93a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c93a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c93a-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="0c93a-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="0c93a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c93a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c93a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c93a-113">Not supported.</span></span>  |
|<span data-ttu-id="0c93a-114">Application</span><span class="sxs-lookup"><span data-stu-id="0c93a-114">Application</span></span> | <span data-ttu-id="0c93a-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="0c93a-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c93a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c93a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c93a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0c93a-117">Optional query parameters</span></span>

<span data-ttu-id="0c93a-118">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="0c93a-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="0c93a-119">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="0c93a-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="0c93a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c93a-120">Request headers</span></span>

| <span data-ttu-id="0c93a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0c93a-121">Name</span></span>      |<span data-ttu-id="0c93a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c93a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0c93a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c93a-123">Authorization</span></span>  | <span data-ttu-id="0c93a-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="0c93a-124">Bearer {code}.</span></span> <span data-ttu-id="0c93a-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c93a-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c93a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c93a-126">Request body</span></span>

<span data-ttu-id="0c93a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c93a-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="0c93a-128">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="0c93a-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="0c93a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c93a-129">Response</span></span>

<span data-ttu-id="0c93a-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScoreControlProfiles** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c93a-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c93a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c93a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c93a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c93a-132">Request</span></span>

<span data-ttu-id="0c93a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c93a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="0c93a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c93a-134">Response</span></span>

<span data-ttu-id="0c93a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c93a-135">The following is an example of the response.</span></span>
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
  "tocPath": ""
}
-->
