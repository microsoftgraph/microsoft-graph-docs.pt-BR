---
title: Listar certificateBasedAuthConfigurations
description: Obtenha uma lista de objetos certificatebasedauthconfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40c4d2f45c9496ffdf8ffc5f0c9fd66373f2db5e
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632541"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="c8401-103">Listar certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="c8401-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="c8401-104">Obtenha uma lista de objetos [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c8401-104">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="c8401-105">Apenas uma única instância do certificateBasedAuthConfiguration pode existir na coleção.</span><span class="sxs-lookup"><span data-stu-id="c8401-105">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="c8401-106">Ele sempre tem uma ID fixa com um valor de ' 29728ade-6ae4-4ee9-9103-412912537da5 '.</span><span class="sxs-lookup"><span data-stu-id="c8401-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8401-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8401-107">Permissions</span></span>

<span data-ttu-id="c8401-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8401-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8401-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8401-110">Permission type</span></span>                        | <span data-ttu-id="c8401-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8401-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8401-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8401-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8401-113">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c8401-113">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="c8401-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8401-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8401-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8401-115">Not supported.</span></span> |
| <span data-ttu-id="c8401-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8401-116">Application</span></span>    | <span data-ttu-id="c8401-117">Organization. Read. All, Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c8401-117">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8401-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8401-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c8401-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8401-119">Request headers</span></span>

| <span data-ttu-id="c8401-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c8401-120">Name</span></span>      |<span data-ttu-id="c8401-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8401-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8401-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8401-122">Authorization</span></span> | <span data-ttu-id="c8401-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8401-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8401-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8401-125">Request body</span></span>

<span data-ttu-id="c8401-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8401-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8401-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8401-127">Response</span></span>

<span data-ttu-id="c8401-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8401-128">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8401-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c8401-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8401-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8401-130">Request</span></span>

<span data-ttu-id="c8401-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8401-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8401-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8401-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8401-133">C#</span><span class="sxs-lookup"><span data-stu-id="c8401-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8401-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8401-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8401-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8401-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8401-136">Java</span><span class="sxs-lookup"><span data-stu-id="c8401-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="c8401-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8401-137">Response</span></span>

<span data-ttu-id="c8401-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8401-138">The following is an example of the response.</span></span>

> <span data-ttu-id="c8401-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8401-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
