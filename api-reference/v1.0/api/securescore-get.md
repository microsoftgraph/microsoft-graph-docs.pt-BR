---
title: Obter secureScore
description: Recupere as propriedades e os relacionamentos de um objeto secureScore.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9b49dde04751aab72eb3c05f9a863cc72df60e7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509861"
---
# <a name="get-securescore"></a><span data-ttu-id="6b322-103">Obter secureScore</span><span class="sxs-lookup"><span data-stu-id="6b322-103">Get secureScore</span></span>

<span data-ttu-id="6b322-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b322-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b322-105">Recupere as propriedades e os relacionamentos de um objeto [secureScore](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="6b322-105">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b322-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b322-106">Permissions</span></span>

<span data-ttu-id="6b322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b322-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b322-109">Permission type</span></span>      | <span data-ttu-id="6b322-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b322-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b322-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b322-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6b322-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b322-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="6b322-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b322-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6b322-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b322-114">Not supported.</span></span>  |
|<span data-ttu-id="6b322-115">Application</span><span class="sxs-lookup"><span data-stu-id="6b322-115">Application</span></span> | <span data-ttu-id="6b322-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b322-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b322-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b322-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6b322-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b322-118">Request headers</span></span>

| <span data-ttu-id="6b322-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b322-119">Name</span></span>      |<span data-ttu-id="6b322-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b322-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b322-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b322-121">Authorization</span></span>  | <span data-ttu-id="6b322-122">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="6b322-122">Bearer {code}.</span></span> <span data-ttu-id="6b322-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b322-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b322-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b322-124">Request body</span></span>

<span data-ttu-id="6b322-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b322-125">Do not supply a request body for this method.</span></span> <span data-ttu-id="6b322-126">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="6b322-126">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="6b322-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b322-127">Response</span></span>

<span data-ttu-id="6b322-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScore** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b322-128">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="6b322-129">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="6b322-129">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="6b322-130">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="6b322-130">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="6b322-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b322-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b322-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b322-132">Request</span></span>

<span data-ttu-id="6b322-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b322-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b322-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b322-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```
# <a name="c"></a>[<span data-ttu-id="6b322-135">C#</span><span class="sxs-lookup"><span data-stu-id="6b322-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b322-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b322-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b322-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b322-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b322-138">Java</span><span class="sxs-lookup"><span data-stu-id="6b322-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b322-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b322-139">Response</span></span>

<span data-ttu-id="6b322-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b322-140">The following is an example of the response.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
