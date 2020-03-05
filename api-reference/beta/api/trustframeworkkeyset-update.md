---
title: Atualizar trustFrameworkKeySet
description: Atualiza as propriedades de um objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc82602e82b1c98fdde2398a576124b563b3c039
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452138"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="ebcdb-103">Atualizar trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="ebcdb-103">Update trustFrameworkKeySet</span></span>

<span data-ttu-id="ebcdb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ebcdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebcdb-105">Atualizar as propriedades de um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="ebcdb-105">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="ebcdb-106">Essa operação substituirá o conteúdo de um conjunto de chaves existente.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-106">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="ebcdb-107">A especificação da ID na carga de solicitação é opcional.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-107">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebcdb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebcdb-108">Permissions</span></span>

<span data-ttu-id="ebcdb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebcdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebcdb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebcdb-111">Permission type</span></span>                        | <span data-ttu-id="ebcdb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebcdb-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ebcdb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebcdb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebcdb-114">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ebcdb-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="ebcdb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebcdb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcdb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-116">Not supported.</span></span> |
| <span data-ttu-id="ebcdb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebcdb-117">Application</span></span>                            | <span data-ttu-id="ebcdb-118">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ebcdb-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebcdb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcdb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ebcdb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcdb-120">Request headers</span></span>

| <span data-ttu-id="ebcdb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ebcdb-121">Name</span></span>       | <span data-ttu-id="ebcdb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcdb-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ebcdb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebcdb-123">Authorization</span></span> | <span data-ttu-id="ebcdb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebcdb-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="ebcdb-126">Content-type</span></span>  | <span data-ttu-id="ebcdb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebcdb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcdb-129">Request body</span></span>


| <span data-ttu-id="ebcdb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebcdb-130">Property</span></span>     | <span data-ttu-id="ebcdb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebcdb-131">Type</span></span>        | <span data-ttu-id="ebcdb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcdb-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ebcdb-133">as</span><span class="sxs-lookup"><span data-stu-id="ebcdb-133">keys</span></span>|<span data-ttu-id="ebcdb-134">coleção [trustFrameworkKey](../resources/trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="ebcdb-134">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="ebcdb-135">atualiza uma coleção de Trustframeworkkeys</span><span class="sxs-lookup"><span data-stu-id="ebcdb-135">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="ebcdb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcdb-136">Response</span></span>

<span data-ttu-id="ebcdb-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-137">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebcdb-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ebcdb-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebcdb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcdb-139">Request</span></span>

<span data-ttu-id="ebcdb-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebcdb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcdb-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_trustframeworkkeyset"
}-->

```http
PUT https://graph.microsoft.com/beta/trustFramework/keySets/{id}
Content-type: application/json

{
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ebcdb-142">C#</span><span class="sxs-lookup"><span data-stu-id="ebcdb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebcdb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebcdb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebcdb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebcdb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ebcdb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcdb-145">Response</span></span>

<span data-ttu-id="ebcdb-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-146">The following is an example of the response.</span></span>

> <span data-ttu-id="ebcdb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebcdb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkkeyset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
