---
title: Obter certificateBasedAuthConfiguration
description: Obter as propriedades de um objeto certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc2c0bd26d18ff8273993b6755ae8809b872f4e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992423"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="6680d-103">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="6680d-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="6680d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6680d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6680d-105">Obter as propriedades de um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6680d-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6680d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6680d-106">Permissions</span></span>

<span data-ttu-id="6680d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6680d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6680d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6680d-109">Permission type</span></span>                        | <span data-ttu-id="6680d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6680d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6680d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6680d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6680d-112">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6680d-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="6680d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6680d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6680d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6680d-114">Not supported.</span></span> |
| <span data-ttu-id="6680d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6680d-115">Application</span></span>    | <span data-ttu-id="6680d-116">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6680d-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6680d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6680d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6680d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6680d-118">Request headers</span></span>

| <span data-ttu-id="6680d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6680d-119">Name</span></span>      |<span data-ttu-id="6680d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6680d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6680d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6680d-121">Authorization</span></span> | <span data-ttu-id="6680d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6680d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6680d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6680d-124">Request body</span></span>

<span data-ttu-id="6680d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6680d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6680d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6680d-126">Response</span></span>

<span data-ttu-id="6680d-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6680d-127">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6680d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6680d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6680d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6680d-129">Request</span></span>

<span data-ttu-id="6680d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6680d-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6680d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6680d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="6680d-132">C#</span><span class="sxs-lookup"><span data-stu-id="6680d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6680d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6680d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6680d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6680d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6680d-135">Java</span><span class="sxs-lookup"><span data-stu-id="6680d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="6680d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6680d-136">Response</span></span>

<span data-ttu-id="6680d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6680d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6680d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6680d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

