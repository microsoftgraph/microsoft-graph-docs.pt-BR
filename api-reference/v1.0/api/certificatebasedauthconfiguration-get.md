---
title: Obter certificateBasedAuthConfiguration
description: Obter as propriedades de um objeto certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 703de60a28c6339556c878b3e53b335bdb4f560c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434829"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="fdeac-103">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fdeac-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="fdeac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdeac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdeac-105">Obter as propriedades de [um objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fdeac-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdeac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdeac-106">Permissions</span></span>

<span data-ttu-id="fdeac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdeac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fdeac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdeac-109">Permission type</span></span>                        | <span data-ttu-id="fdeac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdeac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fdeac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdeac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fdeac-112">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdeac-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="fdeac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdeac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdeac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdeac-114">Not supported.</span></span> |
| <span data-ttu-id="fdeac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdeac-115">Application</span></span>    | <span data-ttu-id="fdeac-116">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdeac-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdeac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdeac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fdeac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdeac-118">Request headers</span></span>

| <span data-ttu-id="fdeac-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fdeac-119">Name</span></span>      |<span data-ttu-id="fdeac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdeac-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fdeac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdeac-121">Authorization</span></span> | <span data-ttu-id="fdeac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdeac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdeac-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdeac-124">Request body</span></span>

<span data-ttu-id="fdeac-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdeac-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdeac-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdeac-126">Response</span></span>

<span data-ttu-id="fdeac-127">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdeac-127">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fdeac-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fdeac-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fdeac-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdeac-129">Request</span></span>

<span data-ttu-id="fdeac-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdeac-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fdeac-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdeac-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="fdeac-132">C#</span><span class="sxs-lookup"><span data-stu-id="fdeac-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdeac-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdeac-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdeac-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdeac-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdeac-135">Java</span><span class="sxs-lookup"><span data-stu-id="fdeac-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="fdeac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdeac-136">Response</span></span>

<span data-ttu-id="fdeac-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fdeac-137">The following is an example of the response.</span></span>

> <span data-ttu-id="fdeac-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdeac-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificateRevocationListUrl": "CRLUrl-value",
      "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

