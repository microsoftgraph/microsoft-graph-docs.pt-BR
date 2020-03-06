---
title: Listar secureScores
description: Recupere uma lista de objetos secureScore.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 75d6865cc1f02dde270bedb40b6c0344d69a4bb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509833"
---
# <a name="list-securescores"></a><span data-ttu-id="81297-103">Listar secureScores</span><span class="sxs-lookup"><span data-stu-id="81297-103">List secureScores</span></span>

<span data-ttu-id="81297-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81297-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81297-105">Recupere uma lista de objetos [secureScore](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="81297-105">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="81297-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81297-106">Permissions</span></span>

<span data-ttu-id="81297-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81297-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81297-109">Permission type</span></span>      | <span data-ttu-id="81297-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81297-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81297-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81297-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="81297-112">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="81297-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="81297-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81297-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="81297-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81297-114">Not supported.</span></span>  |
|<span data-ttu-id="81297-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81297-115">Application</span></span> | <span data-ttu-id="81297-116">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="81297-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81297-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81297-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81297-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81297-118">Optional query parameters</span></span>

<span data-ttu-id="81297-119">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="81297-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="81297-120">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="81297-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="81297-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81297-121">Request headers</span></span>

| <span data-ttu-id="81297-122">Nome</span><span class="sxs-lookup"><span data-stu-id="81297-122">Name</span></span>      |<span data-ttu-id="81297-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="81297-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="81297-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="81297-124">Authorization</span></span>  | <span data-ttu-id="81297-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="81297-125">Bearer {code}.</span></span> <span data-ttu-id="81297-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81297-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81297-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81297-127">Request body</span></span>

<span data-ttu-id="81297-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81297-128">Do not supply a request body for this method.</span></span> <span data-ttu-id="81297-129">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="81297-129">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="81297-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="81297-130">Response</span></span>

<span data-ttu-id="81297-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81297-131">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81297-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81297-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="81297-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81297-133">Request</span></span>

<span data-ttu-id="81297-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81297-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81297-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="81297-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="81297-136">C#</span><span class="sxs-lookup"><span data-stu-id="81297-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81297-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81297-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81297-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81297-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81297-139">Java</span><span class="sxs-lookup"><span data-stu-id="81297-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescores-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81297-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="81297-140">Response</span></span>

<span data-ttu-id="81297-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81297-141">The following is an example of the response.</span></span>
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
