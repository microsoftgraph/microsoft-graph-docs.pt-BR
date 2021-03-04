---
title: Listar certificateBasedAuthConfigurations
description: Obter uma lista de objetos certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6bc1c504ba9acc7f9afeacdf733e572de65f9fca
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437790"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="d1a9f-103">Listar certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="d1a9f-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="d1a9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1a9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1a9f-105">Obter uma lista de [objetos certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1a9f-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="d1a9f-106">Somente uma única instância de certificateBasedAuthConfiguration pode existir na coleção.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="d1a9f-107">Ele sempre tem uma ID fixa com um valor '29728ade-6ae4-4ee9-9103-412912537da5'.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1a9f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1a9f-108">Permissions</span></span>

<span data-ttu-id="d1a9f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1a9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1a9f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1a9f-111">Permission type</span></span>                        | <span data-ttu-id="d1a9f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1a9f-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1a9f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1a9f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1a9f-114">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1a9f-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="d1a9f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1a9f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1a9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-116">Not supported.</span></span> |
| <span data-ttu-id="d1a9f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1a9f-117">Application</span></span>    | <span data-ttu-id="d1a9f-118">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1a9f-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1a9f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1a9f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="d1a9f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a9f-120">Request headers</span></span>

| <span data-ttu-id="d1a9f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d1a9f-121">Name</span></span>      |<span data-ttu-id="d1a9f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1a9f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1a9f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1a9f-123">Authorization</span></span> | <span data-ttu-id="d1a9f-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d1a9f-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1a9f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a9f-125">Request body</span></span>

<span data-ttu-id="d1a9f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1a9f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1a9f-127">Response</span></span>

<span data-ttu-id="d1a9f-128">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-128">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1a9f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1a9f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1a9f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1a9f-130">Request</span></span>

<span data-ttu-id="d1a9f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1a9f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1a9f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="d1a9f-133">C#</span><span class="sxs-lookup"><span data-stu-id="d1a9f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1a9f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1a9f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1a9f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1a9f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1a9f-136">Java</span><span class="sxs-lookup"><span data-stu-id="d1a9f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1a9f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1a9f-137">Response</span></span>

<span data-ttu-id="d1a9f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d1a9f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1a9f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


