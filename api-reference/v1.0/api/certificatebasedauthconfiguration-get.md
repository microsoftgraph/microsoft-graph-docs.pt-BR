---
title: Obter certificateBasedAuthConfiguration
description: Obter as propriedades de um objeto certificatebasedauthconfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d21f7e5824b1144234d2f3371eab53f2f835e4cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632566"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="92063-103">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92063-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="92063-104">Obter as propriedades de um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="92063-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92063-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="92063-105">Permissions</span></span>

<span data-ttu-id="92063-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92063-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92063-108">Permission type</span></span>                        | <span data-ttu-id="92063-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92063-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92063-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92063-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="92063-111">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92063-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="92063-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92063-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92063-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92063-113">Not supported.</span></span> |
| <span data-ttu-id="92063-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92063-114">Application</span></span>    | <span data-ttu-id="92063-115">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92063-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92063-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92063-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92063-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92063-117">Request headers</span></span>

| <span data-ttu-id="92063-118">Nome</span><span class="sxs-lookup"><span data-stu-id="92063-118">Name</span></span>      |<span data-ttu-id="92063-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="92063-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92063-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="92063-120">Authorization</span></span> | <span data-ttu-id="92063-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92063-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92063-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92063-123">Request body</span></span>

<span data-ttu-id="92063-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92063-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92063-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="92063-125">Response</span></span>

<span data-ttu-id="92063-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92063-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92063-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92063-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92063-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92063-128">Request</span></span>

<span data-ttu-id="92063-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92063-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92063-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="92063-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92063-131">C#</span><span class="sxs-lookup"><span data-stu-id="92063-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92063-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92063-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92063-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92063-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92063-134">Java</span><span class="sxs-lookup"><span data-stu-id="92063-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="92063-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="92063-135">Response</span></span>

<span data-ttu-id="92063-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92063-136">The following is an example of the response.</span></span>

> <span data-ttu-id="92063-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92063-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
