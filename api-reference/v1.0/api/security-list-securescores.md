---
title: Listar secureScores
description: Recupere uma lista de objetos secureScore.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 16e2967046797abce4ee04e7a8fae4d451447823
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025407"
---
# <a name="list-securescores"></a><span data-ttu-id="f0f5b-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="f0f5b-103">List secureScores</span></span>

<span data-ttu-id="f0f5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0f5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0f5b-105">Recupere uma lista de objetos [secureScore](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="f0f5b-105">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0f5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0f5b-106">Permissions</span></span>

<span data-ttu-id="f0f5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0f5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0f5b-109">Permission type</span></span>      | <span data-ttu-id="f0f5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0f5b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0f5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0f5b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f0f5b-112">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="f0f5b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0f5b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f0f5b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-114">Not supported.</span></span>  |
|<span data-ttu-id="f0f5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0f5b-115">Application</span></span> | <span data-ttu-id="f0f5b-116">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0f5b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0f5b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0f5b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0f5b-118">Optional query parameters</span></span>

<span data-ttu-id="f0f5b-119">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="f0f5b-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="f0f5b-120">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="f0f5b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f5b-121">Request headers</span></span>

| <span data-ttu-id="f0f5b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f0f5b-122">Name</span></span>      |<span data-ttu-id="f0f5b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0f5b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0f5b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0f5b-124">Authorization</span></span>  | <span data-ttu-id="f0f5b-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-125">Bearer {code}.</span></span> <span data-ttu-id="f0f5b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f5b-127">Request body</span></span>

<span data-ttu-id="f0f5b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-128">Do not supply a request body for this method.</span></span> <span data-ttu-id="f0f5b-129">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-129">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="f0f5b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f5b-130">Response</span></span>

<span data-ttu-id="f0f5b-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-131">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f5b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0f5b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0f5b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f5b-133">Request</span></span>

<span data-ttu-id="f0f5b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0f5b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0f5b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="f0f5b-136">C#</span><span class="sxs-lookup"><span data-stu-id="f0f5b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0f5b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0f5b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0f5b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0f5b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0f5b-139">Java</span><span class="sxs-lookup"><span data-stu-id="f0f5b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescores-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0f5b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f5b-140">Response</span></span>

<span data-ttu-id="f0f5b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0f5b-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
            "azureTenantId": "00000001-0001-0001-0001-000000000001c",
            "activeUserCount": 0,
            "createdDateTime": "2019-03-19T15:21:00Z",
            "currentScore": 387.0,
            "enabledServices": [
                "HasExchange",
                "HasSharePoint",
                "HasInTune"
            ],
            "licensedUserCount": 100,
            "maxScore": 697.0,
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": 37.0
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": 46.0
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": 109.0
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "Identity",
                    "controlName": "AdminMFA",
                    "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
                    "score": 35.0
                },
                {
                    "controlCategory": "Data",
                    "controlName": "DLPEnabled",
                    "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
                    "score": 20.0
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
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

