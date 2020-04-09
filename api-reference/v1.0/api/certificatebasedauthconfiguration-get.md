---
title: Obter certificateBasedAuthConfiguration
description: Obter as propriedades de um objeto certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 232dc629fdd4e6bec1914654d036c8d097d2bd17
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181256"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="210d1-103">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="210d1-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="210d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="210d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="210d1-105">Obter as propriedades de um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="210d1-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="210d1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="210d1-106">Permissions</span></span>

<span data-ttu-id="210d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="210d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="210d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="210d1-109">Permission type</span></span>                        | <span data-ttu-id="210d1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="210d1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="210d1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="210d1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="210d1-112">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="210d1-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="210d1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="210d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="210d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="210d1-114">Not supported.</span></span> |
| <span data-ttu-id="210d1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="210d1-115">Application</span></span>    | <span data-ttu-id="210d1-116">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="210d1-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="210d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="210d1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="210d1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="210d1-118">Request headers</span></span>

| <span data-ttu-id="210d1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="210d1-119">Name</span></span>      |<span data-ttu-id="210d1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="210d1-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="210d1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="210d1-121">Authorization</span></span> | <span data-ttu-id="210d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="210d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="210d1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="210d1-124">Request body</span></span>

<span data-ttu-id="210d1-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="210d1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="210d1-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="210d1-126">Response</span></span>

<span data-ttu-id="210d1-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="210d1-127">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="210d1-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="210d1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="210d1-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="210d1-129">Request</span></span>

<span data-ttu-id="210d1-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="210d1-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="210d1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="210d1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="210d1-132">C#</span><span class="sxs-lookup"><span data-stu-id="210d1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="210d1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="210d1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="210d1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="210d1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="210d1-135">Java</span><span class="sxs-lookup"><span data-stu-id="210d1-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="210d1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="210d1-136">Response</span></span>

<span data-ttu-id="210d1-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="210d1-137">The following is an example of the response.</span></span>

> <span data-ttu-id="210d1-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="210d1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
