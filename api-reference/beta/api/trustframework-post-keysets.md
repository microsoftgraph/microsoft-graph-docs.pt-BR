---
title: Criar trustFrameworkKeySet
description: Crie um novo **objeto trustFrameworkKeySet.**
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 909198910f311053af9cca71c1dae34beb65e13c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053444"
---
# <a name="create-trustframeworkkeyset"></a><span data-ttu-id="d630e-103">Criar trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="d630e-103">Create trustFrameworkKeySet</span></span>

<span data-ttu-id="d630e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d630e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d630e-105">Crie um novo [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="d630e-105">Create a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="d630e-106">A ID do **trustFrameworkKeySet** é esperada na solicitação de criação; no entanto, ele pode ser modificado pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="d630e-106">The ID of the **trustFrameworkKeySet** is expected in the create request; however, it can be modified by the service.</span></span> <span data-ttu-id="d630e-107">A ID modificada estará disponível na resposta e no header de local.</span><span class="sxs-lookup"><span data-stu-id="d630e-107">The modified ID will be available in the response and in the location header.</span></span>

## <a name="permissions"></a><span data-ttu-id="d630e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d630e-108">Permissions</span></span>

<span data-ttu-id="d630e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d630e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d630e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d630e-111">Permission type</span></span>                        | <span data-ttu-id="d630e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d630e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d630e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d630e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d630e-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d630e-114">TrustFrameworkKeySet.ReadWrite.All</span></span>   |
| <span data-ttu-id="d630e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d630e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d630e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d630e-116">Not supported.</span></span> |
| <span data-ttu-id="d630e-117">Application</span><span class="sxs-lookup"><span data-stu-id="d630e-117">Application</span></span>                            | <span data-ttu-id="d630e-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d630e-118">TrustFrameworkKeySet.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="d630e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d630e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="d630e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d630e-120">Request headers</span></span>

| <span data-ttu-id="d630e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d630e-121">Name</span></span>          | <span data-ttu-id="d630e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d630e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d630e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d630e-123">Authorization</span></span> | <span data-ttu-id="d630e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d630e-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d630e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d630e-126">Content-type</span></span> | <span data-ttu-id="d630e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d630e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d630e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d630e-129">Request body</span></span>

<span data-ttu-id="d630e-130">No corpo da solicitação, fornece uma representação JSON de um [objeto trustFrameworkKeySet.](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="d630e-130">In the request body, supply a JSON representation of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d630e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d630e-131">Response</span></span>

<span data-ttu-id="d630e-132">Se tiver êxito, este método retornará um código de resposta, um header de local para o objeto recém-criado e um novo `201 Created` [objeto trustFrameworkKeySet](../resources/trustframeworkkeyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d630e-132">If successful, this method returns a `201 Created` response code, a location header for the newly created object, and a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d630e-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d630e-133">Examples</span></span>

### <a name="example-1-create-an-empty-keyset"></a><span data-ttu-id="d630e-134">Exemplo 1: Criar um keyset vazio</span><span class="sxs-lookup"><span data-stu-id="d630e-134">Example 1: Create an empty keyset</span></span>
<span data-ttu-id="d630e-135">Esta é uma das operações mais úteis.</span><span class="sxs-lookup"><span data-stu-id="d630e-135">This is one of the most useful operations.</span></span> <span data-ttu-id="d630e-136">Primeiro, você cria um keyset vazio.</span><span class="sxs-lookup"><span data-stu-id="d630e-136">First, you create an empty keyset.</span></span> <span data-ttu-id="d630e-137">Em seguida, no novo keyset, você pode gerar uma chave, carregar um segredo manual e carregar um certificado ou uma tecla PKCS12.</span><span class="sxs-lookup"><span data-stu-id="d630e-137">Then, in the new keyset, you can generate a key, upload a manual secret, and upload a certificate or a PKCS12 key.</span></span> 

#### <a name="request"></a><span data-ttu-id="d630e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d630e-138">Request</span></span>

<span data-ttu-id="d630e-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d630e-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d630e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d630e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework1"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1"  
}
```
# <a name="c"></a>[<span data-ttu-id="d630e-141">C#</span><span class="sxs-lookup"><span data-stu-id="d630e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-trustframeworkkeyset-from-trustframework-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d630e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d630e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-trustframeworkkeyset-from-trustframework-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d630e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d630e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-trustframeworkkeyset-from-trustframework-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d630e-144">Java</span><span class="sxs-lookup"><span data-stu-id="d630e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-trustframeworkkeyset-from-trustframework-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d630e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d630e-145">Response</span></span>

<span data-ttu-id="d630e-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="d630e-146">The following example shows the response.</span></span>

> <span data-ttu-id="d630e-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d630e-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
  "keys": []
}
```

### <a name="example-2-create-a-keyset-with-a-key"></a><span data-ttu-id="d630e-148">Exemplo 2: Criar um keyset com uma chave</span><span class="sxs-lookup"><span data-stu-id="d630e-148">Example 2: Create a keyset with a key</span></span>

<span data-ttu-id="d630e-149">Este é um cenário avançado em que você precisa saber o formato JSON Web Key compatível com [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) da chave.</span><span class="sxs-lookup"><span data-stu-id="d630e-149">This is an advanced scenario where you need to know the [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) compliant JSON Web Key format of the key.</span></span>

#### <a name="request"></a><span data-ttu-id="d630e-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d630e-150">Request</span></span>

<span data-ttu-id="d630e-151">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d630e-151">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1",
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

#### <a name="response"></a><span data-ttu-id="d630e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d630e-152">Response</span></span>

<span data-ttu-id="d630e-153">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="d630e-153">The following example shows the response.</span></span>

> <span data-ttu-id="d630e-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d630e-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
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
  "description": "Create trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


