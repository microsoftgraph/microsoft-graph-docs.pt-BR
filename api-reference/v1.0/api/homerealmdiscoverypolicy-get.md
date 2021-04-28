---
title: Obter homeRealmDiscoveryPolicy
description: Recupere as propriedades e as relações do objeto homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bdd96dbd20429e0175f2d075f5e0abf6a95b764c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039591"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="74958-103">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="74958-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="74958-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74958-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="74958-105">Recupere as propriedades e as relações de um [objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74958-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74958-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="74958-106">Permissions</span></span>

<span data-ttu-id="74958-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74958-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74958-109">Permission type</span></span>                        | <span data-ttu-id="74958-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74958-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74958-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74958-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="74958-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="74958-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="74958-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74958-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74958-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74958-114">Not supported.</span></span> |
| <span data-ttu-id="74958-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74958-115">Application</span></span>                            | <span data-ttu-id="74958-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="74958-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="74958-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74958-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74958-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74958-118">Optional query parameters</span></span>

<span data-ttu-id="74958-119">Este método dá suporte aos `$expand` `$select` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74958-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="74958-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="74958-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="74958-121">Ao usar `$expand` , certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="74958-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74958-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74958-122">Request headers</span></span>

| <span data-ttu-id="74958-123">Nome</span><span class="sxs-lookup"><span data-stu-id="74958-123">Name</span></span>      |<span data-ttu-id="74958-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="74958-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="74958-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="74958-125">Authorization</span></span> | <span data-ttu-id="74958-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74958-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74958-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74958-128">Request body</span></span>

<span data-ttu-id="74958-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74958-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74958-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="74958-130">Response</span></span>

<span data-ttu-id="74958-131">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74958-131">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74958-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="74958-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74958-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74958-133">Request</span></span>

<span data-ttu-id="74958-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74958-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="74958-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="74958-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="74958-136">C#</span><span class="sxs-lookup"><span data-stu-id="74958-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74958-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74958-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74958-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74958-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74958-139">Java</span><span class="sxs-lookup"><span data-stu-id="74958-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74958-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="74958-140">Response</span></span>

<span data-ttu-id="74958-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74958-141">The following is an example of the response.</span></span>

> <span data-ttu-id="74958-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74958-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

