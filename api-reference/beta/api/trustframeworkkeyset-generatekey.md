---
title: 'trustFrameworkKeySet: generateKey'
description: Gere uma chave e um segredo automaticamente no keyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6ffcb8beb1744d8ca702ed1d9fd550721b6e7747
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433642"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="122b8-103">trustFrameworkKeySet: generateKey</span><span class="sxs-lookup"><span data-stu-id="122b8-103">trustFrameworkKeySet: generateKey</span></span>

<span data-ttu-id="122b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="122b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="122b8-105">Gere [um trustFrameworkKey](../resources/trustFrameworkKey.md) e um segredo automaticamente [no trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="122b8-105">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="122b8-106">O chamador não precisa fornecer um segredo.</span><span class="sxs-lookup"><span data-stu-id="122b8-106">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="122b8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="122b8-107">Permissions</span></span>

<span data-ttu-id="122b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="122b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="122b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="122b8-110">Permission type</span></span>                        | <span data-ttu-id="122b8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="122b8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="122b8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="122b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="122b8-113">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="122b8-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="122b8-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="122b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="122b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="122b8-115">Not supported.</span></span> |
| <span data-ttu-id="122b8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="122b8-116">Application</span></span>                            | <span data-ttu-id="122b8-117">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="122b8-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="122b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="122b8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="122b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="122b8-119">Request headers</span></span>

| <span data-ttu-id="122b8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="122b8-120">Name</span></span>          | <span data-ttu-id="122b8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="122b8-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="122b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="122b8-122">Authorization</span></span> | <span data-ttu-id="122b8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="122b8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="122b8-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="122b8-125">Content-type</span></span>  | <span data-ttu-id="122b8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="122b8-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="122b8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="122b8-128">Request body</span></span>

<span data-ttu-id="122b8-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="122b8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="122b8-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="122b8-130">Parameter</span></span>    | <span data-ttu-id="122b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="122b8-131">Type</span></span>        | <span data-ttu-id="122b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="122b8-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="122b8-133">use</span><span class="sxs-lookup"><span data-stu-id="122b8-133">use</span></span> | <span data-ttu-id="122b8-134">string</span><span class="sxs-lookup"><span data-stu-id="122b8-134">string</span></span> | <span data-ttu-id="122b8-135">Semelhante à propriedade **use** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="122b8-135">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="122b8-136">kty</span><span class="sxs-lookup"><span data-stu-id="122b8-136">kty</span></span> | <span data-ttu-id="122b8-137">string</span><span class="sxs-lookup"><span data-stu-id="122b8-137">string</span></span> | <span data-ttu-id="122b8-138">Semelhante à **propriedade kty** **de trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="122b8-138">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="122b8-139">nbf</span><span class="sxs-lookup"><span data-stu-id="122b8-139">nbf</span></span> | <span data-ttu-id="122b8-140">int</span><span class="sxs-lookup"><span data-stu-id="122b8-140">int</span></span> | <span data-ttu-id="122b8-141">Semelhante à **propriedade nbf** **de trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="122b8-141">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="122b8-142">exp</span><span class="sxs-lookup"><span data-stu-id="122b8-142">exp</span></span> | <span data-ttu-id="122b8-143">int</span><span class="sxs-lookup"><span data-stu-id="122b8-143">int</span></span> | <span data-ttu-id="122b8-144">Semelhante à **propriedade exp** **de trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="122b8-144">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="122b8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="122b8-145">Response</span></span>

<span data-ttu-id="122b8-146">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="122b8-146">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="122b8-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="122b8-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="122b8-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="122b8-148">Request</span></span>

<span data-ttu-id="122b8-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="122b8-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="122b8-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="122b8-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_generatekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/generateKey
Content-type: application/json

{
  "use": "sig",
  "kty": "RSA",
  "nbf": 1508969811,
  "exp": 1508969811
}
```
# <a name="c"></a>[<span data-ttu-id="122b8-151">C#</span><span class="sxs-lookup"><span data-stu-id="122b8-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="122b8-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="122b8-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="122b8-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="122b8-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="122b8-154">Java</span><span class="sxs-lookup"><span data-stu-id="122b8-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-generatekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="122b8-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="122b8-155">Response</span></span>

<span data-ttu-id="122b8-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="122b8-156">The following is an example of the response.</span></span>

> <span data-ttu-id="122b8-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="122b8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.trustFrameworkKey",
    "k": null,
    "x5c": [],
    "kty": "RSA",
    "use": "sig",
    "exp": 1908969811,
    "nbf": 1908969811,
    "kid": "Gaid7K8sO8RavMX9fzHir_Wg0femGhbY9b-B4rVIxbE",
    "e": "AQAB",
    "n": "rd54s6",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: generateKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


