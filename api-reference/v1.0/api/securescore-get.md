---
title: Obter secureScore
description: Recupere as propriedades e os relacionamentos de um objeto secureScore.
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 22bdce327d8f14bf338efc4f5bad709819a6421c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951297"
---
# <a name="get-securescore"></a><span data-ttu-id="b489b-103">Obter secureScore</span><span class="sxs-lookup"><span data-stu-id="b489b-103">Get secureScore</span></span>

<span data-ttu-id="b489b-104">Recupere as propriedades e os relacionamentos de um objeto [secureScore](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="b489b-104">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b489b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b489b-105">Permissions</span></span>

<span data-ttu-id="b489b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b489b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b489b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b489b-108">Permission type</span></span>      | <span data-ttu-id="b489b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b489b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b489b-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b489b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b489b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b489b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="b489b-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b489b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b489b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b489b-113">Not supported.</span></span>  |
|<span data-ttu-id="b489b-114">Application</span><span class="sxs-lookup"><span data-stu-id="b489b-114">Application</span></span> | <span data-ttu-id="b489b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b489b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b489b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b489b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b489b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b489b-117">Request headers</span></span>

| <span data-ttu-id="b489b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b489b-118">Name</span></span>      |<span data-ttu-id="b489b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b489b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b489b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b489b-120">Authorization</span></span>  | <span data-ttu-id="b489b-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="b489b-121">Bearer {code}.</span></span> <span data-ttu-id="b489b-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b489b-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b489b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b489b-123">Request body</span></span>

<span data-ttu-id="b489b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b489b-124">Do not supply a request body for this method.</span></span> <span data-ttu-id="b489b-125">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="b489b-125">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="b489b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b489b-126">Response</span></span>

<span data-ttu-id="b489b-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScore** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b489b-127">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="b489b-128">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="b489b-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="b489b-129">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="b489b-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="b489b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b489b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b489b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b489b-131">Request</span></span>

<span data-ttu-id="b489b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b489b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```

### <a name="response"></a><span data-ttu-id="b489b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b489b-133">Response</span></span>

<span data-ttu-id="b489b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b489b-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b489b-135">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="b489b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b489b-136">C#</span><span class="sxs-lookup"><span data-stu-id="b489b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescore-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b489b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b489b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescore-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
