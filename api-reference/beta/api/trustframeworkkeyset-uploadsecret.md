---
title: 'trustFrameworkKeySet: uploadSecret'
description: Carregue um segredo em um keyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b008e1ae41d61fb14dbd80e5a820208355bb670d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444970"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="f7476-103">trustFrameworkKeySet: uploadSecret</span><span class="sxs-lookup"><span data-stu-id="f7476-103">trustFrameworkKeySet: uploadSecret</span></span>

<span data-ttu-id="f7476-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7476-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7476-105">Carregue um segredo de texto simples em [um trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="f7476-105">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="f7476-106">Exemplos de segredos são segredos de aplicativos no Azure Active Directory, Google, Facebook ou qualquer outro provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="f7476-106">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="f7476-107">seu método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="f7476-107">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7476-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7476-108">Permissions</span></span>

<span data-ttu-id="f7476-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7476-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7476-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7476-111">Permission type</span></span>                        | <span data-ttu-id="f7476-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7476-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7476-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7476-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7476-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7476-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="f7476-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7476-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7476-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7476-116">Not supported.</span></span> |
| <span data-ttu-id="f7476-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7476-117">Application</span></span>                            | <span data-ttu-id="f7476-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7476-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7476-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7476-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="f7476-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7476-120">Request headers</span></span>

| <span data-ttu-id="f7476-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f7476-121">Name</span></span>          | <span data-ttu-id="f7476-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7476-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7476-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7476-123">Authorization</span></span> | <span data-ttu-id="f7476-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7476-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7476-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f7476-126">Content-type</span></span>  | <span data-ttu-id="f7476-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7476-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7476-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7476-129">Request body</span></span>

<span data-ttu-id="f7476-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7476-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7476-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f7476-131">Parameter</span></span>    | <span data-ttu-id="f7476-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7476-132">Type</span></span>        | <span data-ttu-id="f7476-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7476-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7476-134">use</span><span class="sxs-lookup"><span data-stu-id="f7476-134">use</span></span>|<span data-ttu-id="f7476-135">String</span><span class="sxs-lookup"><span data-stu-id="f7476-135">String</span></span>|<span data-ttu-id="f7476-136">Semelhante à propriedade **use** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="f7476-136">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="f7476-137">k</span><span class="sxs-lookup"><span data-stu-id="f7476-137">k</span></span>|<span data-ttu-id="f7476-138">String</span><span class="sxs-lookup"><span data-stu-id="f7476-138">String</span></span>|<span data-ttu-id="f7476-139">Semelhante à propriedade **k** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="f7476-139">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="f7476-140">Este é o campo usado para enviar o segredo.</span><span class="sxs-lookup"><span data-stu-id="f7476-140">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="f7476-141">nbf</span><span class="sxs-lookup"><span data-stu-id="f7476-141">nbf</span></span>|<span data-ttu-id="f7476-142">Int64</span><span class="sxs-lookup"><span data-stu-id="f7476-142">Int64</span></span>|<span data-ttu-id="f7476-143">Semelhante à propriedade **nbf** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="f7476-143">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="f7476-144">exp</span><span class="sxs-lookup"><span data-stu-id="f7476-144">exp</span></span>|<span data-ttu-id="f7476-145">Int64</span><span class="sxs-lookup"><span data-stu-id="f7476-145">Int64</span></span>|<span data-ttu-id="f7476-146">Semelhante à propriedade **exp** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="f7476-146">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="f7476-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7476-147">Response</span></span>

<span data-ttu-id="f7476-148">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7476-148">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7476-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7476-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7476-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7476-150">Request</span></span>

<span data-ttu-id="f7476-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7476-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7476-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7476-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadsecret"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadSecret
Content-type: application/json

{
  "use": "use-value",
  "k": "application-secret-to-be-uploaded",
  "nbf": 1508969811,
  "exp": 1508973711
}
```
# <a name="c"></a>[<span data-ttu-id="f7476-153">C#</span><span class="sxs-lookup"><span data-stu-id="f7476-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7476-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7476-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7476-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7476-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7476-156">Java</span><span class="sxs-lookup"><span data-stu-id="f7476-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadsecret-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7476-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7476-157">Response</span></span>

<span data-ttu-id="f7476-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7476-158">The following is an example of the response.</span></span>

> <span data-ttu-id="f7476-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7476-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "use-value",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadSecret",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


