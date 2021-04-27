---
title: Obter certificateBasedAuthConfiguration
description: Obter as propriedades de um objeto certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5009db18fd17ae160375f76db296f1d3f5a9c694
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047571"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="0e169-103">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e169-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="0e169-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e169-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e169-105">Obter as propriedades de [um objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e169-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e169-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e169-106">Permissions</span></span>

<span data-ttu-id="0e169-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e169-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e169-109">Permission type</span></span>                        | <span data-ttu-id="0e169-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e169-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e169-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e169-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e169-112">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e169-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="0e169-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e169-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e169-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e169-114">Not supported.</span></span> |
| <span data-ttu-id="0e169-115">Application</span><span class="sxs-lookup"><span data-stu-id="0e169-115">Application</span></span>    | <span data-ttu-id="0e169-116">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e169-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e169-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e169-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e169-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e169-118">Request headers</span></span>

| <span data-ttu-id="0e169-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0e169-119">Name</span></span>      |<span data-ttu-id="0e169-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e169-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e169-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e169-121">Authorization</span></span> | <span data-ttu-id="0e169-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0e169-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e169-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e169-123">Request body</span></span>

<span data-ttu-id="0e169-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e169-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e169-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e169-125">Response</span></span>

<span data-ttu-id="0e169-126">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e169-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e169-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0e169-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e169-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e169-128">Request</span></span>

<span data-ttu-id="0e169-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e169-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e169-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e169-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="0e169-131">C#</span><span class="sxs-lookup"><span data-stu-id="0e169-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e169-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e169-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e169-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e169-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e169-134">Java</span><span class="sxs-lookup"><span data-stu-id="0e169-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e169-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e169-135">Response</span></span>

<span data-ttu-id="0e169-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e169-136">The following is an example of the response.</span></span>

> <span data-ttu-id="0e169-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0e169-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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


