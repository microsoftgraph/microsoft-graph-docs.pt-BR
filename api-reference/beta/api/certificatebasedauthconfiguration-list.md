---
title: Listar certificateBasedAuthConfigurations
description: Obtenha uma lista de objetos certificatebasedauthconfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 738845b92731df7090754301d90e01049810d072
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718678"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="ff998-103">Listar certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="ff998-103">List certificateBasedAuthConfigurations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff998-104">Obtenha uma lista de objetos [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ff998-104">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="ff998-105">Apenas uma única instância do certificateBasedAuthConfiguration pode existir na coleção.</span><span class="sxs-lookup"><span data-stu-id="ff998-105">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="ff998-106">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="ff998-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff998-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff998-107">Permissions</span></span>

<span data-ttu-id="ff998-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff998-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff998-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff998-110">Permission type</span></span>                        | <span data-ttu-id="ff998-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff998-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff998-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff998-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff998-113">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ff998-113">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="ff998-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff998-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff998-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff998-115">Not supported.</span></span> |
| <span data-ttu-id="ff998-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff998-116">Application</span></span>    | <span data-ttu-id="ff998-117">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ff998-117">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff998-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff998-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="ff998-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff998-119">Request headers</span></span>

| <span data-ttu-id="ff998-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ff998-120">Name</span></span>      |<span data-ttu-id="ff998-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff998-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff998-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff998-122">Authorization</span></span> | <span data-ttu-id="ff998-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ff998-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff998-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff998-124">Request body</span></span>

<span data-ttu-id="ff998-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff998-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff998-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff998-126">Response</span></span>

<span data-ttu-id="ff998-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff998-127">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff998-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff998-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff998-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff998-129">Request</span></span>

<span data-ttu-id="ff998-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff998-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff998-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff998-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff998-132">C#</span><span class="sxs-lookup"><span data-stu-id="ff998-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff998-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff998-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff998-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff998-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff998-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff998-135">Response</span></span>

<span data-ttu-id="ff998-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff998-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ff998-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff998-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
