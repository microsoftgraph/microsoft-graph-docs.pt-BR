---
title: Listar secureScores
description: Recupere uma lista de objetos secureScore.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: ba63b8b6043c2079943b83be46227c31a197dce9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273164"
---
# <a name="list-securescores"></a><span data-ttu-id="69f3e-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="69f3e-103">List secureScores</span></span>

<span data-ttu-id="69f3e-104">Recupere uma lista de objetos [secureScore](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="69f3e-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="69f3e-105">Permissions</span></span>

<span data-ttu-id="69f3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69f3e-108">Permission type</span></span>      | <span data-ttu-id="69f3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69f3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69f3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69f3e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="69f3e-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="69f3e-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="69f3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69f3e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="69f3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69f3e-113">Not supported.</span></span>  |
|<span data-ttu-id="69f3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69f3e-114">Application</span></span> | <span data-ttu-id="69f3e-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="69f3e-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69f3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69f3e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69f3e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="69f3e-117">Optional query parameters</span></span>

<span data-ttu-id="69f3e-118">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="69f3e-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="69f3e-119">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="69f3e-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="69f3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69f3e-120">Request headers</span></span>

| <span data-ttu-id="69f3e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="69f3e-121">Name</span></span>      |<span data-ttu-id="69f3e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f3e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="69f3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="69f3e-123">Authorization</span></span>  | <span data-ttu-id="69f3e-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="69f3e-124">Bearer {code}.</span></span> <span data-ttu-id="69f3e-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69f3e-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69f3e-126">Request body</span></span>

<span data-ttu-id="69f3e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69f3e-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="69f3e-128">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="69f3e-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="69f3e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f3e-129">Response</span></span>

<span data-ttu-id="69f3e-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69f3e-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f3e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69f3e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f3e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69f3e-132">Request</span></span>

<span data-ttu-id="69f3e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69f3e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="69f3e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="69f3e-134">Response</span></span>

<span data-ttu-id="69f3e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69f3e-135">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="69f3e-136">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="69f3e-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="69f3e-137">C#</span><span class="sxs-lookup"><span data-stu-id="69f3e-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescores-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69f3e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="69f3e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescores-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="69f3e-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="69f3e-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_securescores-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
