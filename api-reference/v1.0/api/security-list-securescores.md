---
title: Listar secureScores
description: Recupere uma lista de objetos secureScore.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8210f96b4db8a05efc2fa1c82c384ec822c4afb1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307872"
---
# <a name="list-securescores"></a><span data-ttu-id="118bf-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="118bf-103">List secureScores</span></span>

<span data-ttu-id="118bf-104">Recupere uma lista de objetos [secureScore](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="118bf-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="118bf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="118bf-105">Permissions</span></span>

<span data-ttu-id="118bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="118bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="118bf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="118bf-108">Permission type</span></span>      | <span data-ttu-id="118bf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="118bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="118bf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="118bf-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="118bf-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="118bf-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="118bf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="118bf-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="118bf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="118bf-113">Not supported.</span></span>  |
|<span data-ttu-id="118bf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="118bf-114">Application</span></span> | <span data-ttu-id="118bf-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="118bf-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="118bf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="118bf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="118bf-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="118bf-117">Optional query parameters</span></span>

<span data-ttu-id="118bf-118">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="118bf-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="118bf-119">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="118bf-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="118bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="118bf-120">Request headers</span></span>

| <span data-ttu-id="118bf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="118bf-121">Name</span></span>      |<span data-ttu-id="118bf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="118bf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="118bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="118bf-123">Authorization</span></span>  | <span data-ttu-id="118bf-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="118bf-124">Bearer {code}.</span></span> <span data-ttu-id="118bf-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="118bf-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="118bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="118bf-126">Request body</span></span>

<span data-ttu-id="118bf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="118bf-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="118bf-128">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="118bf-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="118bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="118bf-129">Response</span></span>

<span data-ttu-id="118bf-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="118bf-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="118bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="118bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="118bf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="118bf-132">Request</span></span>

<span data-ttu-id="118bf-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="118bf-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="118bf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="118bf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="118bf-135">C#</span><span class="sxs-lookup"><span data-stu-id="118bf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="118bf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="118bf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="118bf-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="118bf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="118bf-138">Java</span><span class="sxs-lookup"><span data-stu-id="118bf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescores-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="118bf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="118bf-139">Response</span></span>

<span data-ttu-id="118bf-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="118bf-140">The following is an example of the response.</span></span>
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
