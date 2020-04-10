---
title: 'trustFrameworkKeySet: generateKey'
description: Gerar uma chave e um segredo automaticamente no conjunto de chaves.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8c3385a06c8807ce82169efb5a02f1999223cd4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215931"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="d1caf-103">trustFrameworkKeySet: generateKey</span><span class="sxs-lookup"><span data-stu-id="d1caf-103">trustFrameworkKeySet: generateKey</span></span>

<span data-ttu-id="d1caf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1caf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1caf-105">Gere um [trustFrameworkKey](../resources/trustFrameworkKey.md) e um segredo automaticamente no [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="d1caf-105">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="d1caf-106">O chamador não precisa fornecer um segredo.</span><span class="sxs-lookup"><span data-stu-id="d1caf-106">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1caf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1caf-107">Permissions</span></span>

<span data-ttu-id="d1caf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1caf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1caf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1caf-110">Permission type</span></span>                        | <span data-ttu-id="d1caf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1caf-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1caf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1caf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1caf-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d1caf-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="d1caf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1caf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1caf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1caf-115">Not supported.</span></span> |
| <span data-ttu-id="d1caf-116">Application</span><span class="sxs-lookup"><span data-stu-id="d1caf-116">Application</span></span>                            | <span data-ttu-id="d1caf-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d1caf-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1caf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1caf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="d1caf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1caf-119">Request headers</span></span>

| <span data-ttu-id="d1caf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d1caf-120">Name</span></span>          | <span data-ttu-id="d1caf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1caf-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d1caf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1caf-122">Authorization</span></span> | <span data-ttu-id="d1caf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1caf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1caf-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="d1caf-125">Content-type</span></span>  | <span data-ttu-id="d1caf-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1caf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1caf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1caf-128">Request body</span></span>

<span data-ttu-id="d1caf-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1caf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1caf-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d1caf-130">Parameter</span></span>    | <span data-ttu-id="d1caf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1caf-131">Type</span></span>        | <span data-ttu-id="d1caf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1caf-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d1caf-133">Use</span><span class="sxs-lookup"><span data-stu-id="d1caf-133">use</span></span> | <span data-ttu-id="d1caf-134">string</span><span class="sxs-lookup"><span data-stu-id="d1caf-134">string</span></span> | <span data-ttu-id="d1caf-135">Semelhante à propriedade **use** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="d1caf-135">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="d1caf-136">kty</span><span class="sxs-lookup"><span data-stu-id="d1caf-136">kty</span></span> | <span data-ttu-id="d1caf-137">string</span><span class="sxs-lookup"><span data-stu-id="d1caf-137">string</span></span> | <span data-ttu-id="d1caf-138">Semelhante à propriedade **KTY** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="d1caf-138">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="d1caf-139">nbf</span><span class="sxs-lookup"><span data-stu-id="d1caf-139">nbf</span></span> | <span data-ttu-id="d1caf-140">int</span><span class="sxs-lookup"><span data-stu-id="d1caf-140">int</span></span> | <span data-ttu-id="d1caf-141">Semelhante à propriedade **NBF** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="d1caf-141">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="d1caf-142">exp</span><span class="sxs-lookup"><span data-stu-id="d1caf-142">exp</span></span> | <span data-ttu-id="d1caf-143">int</span><span class="sxs-lookup"><span data-stu-id="d1caf-143">int</span></span> | <span data-ttu-id="d1caf-144">Semelhante à propriedade **exp** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="d1caf-144">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="d1caf-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1caf-145">Response</span></span>

<span data-ttu-id="d1caf-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1caf-146">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1caf-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1caf-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1caf-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1caf-148">Request</span></span>

<span data-ttu-id="d1caf-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1caf-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1caf-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1caf-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d1caf-151">C#</span><span class="sxs-lookup"><span data-stu-id="d1caf-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1caf-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1caf-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1caf-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1caf-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1caf-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1caf-154">Response</span></span>

<span data-ttu-id="d1caf-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1caf-155">The following is an example of the response.</span></span>

> <span data-ttu-id="d1caf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1caf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
