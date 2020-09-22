---
title: 'trustFrameworkKeySet: uploadSecret'
description: Carregar um segredo em um conjunto de chaves.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82d45f8af4e9a7a80626ad83c58b4fa58c5bb5de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095664"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="0ebff-103">trustFrameworkKeySet: uploadSecret</span><span class="sxs-lookup"><span data-stu-id="0ebff-103">trustFrameworkKeySet: uploadSecret</span></span>

<span data-ttu-id="0ebff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ebff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ebff-105">Carregar um segredo de texto sem formatação em um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="0ebff-105">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="0ebff-106">Exemplos de segredos são segredos do aplicativo no Azure Active Directory, Google, Facebook ou qualquer outro provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="0ebff-106">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="0ebff-107">o método his retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="0ebff-107">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ebff-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ebff-108">Permissions</span></span>

<span data-ttu-id="0ebff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ebff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ebff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ebff-111">Permission type</span></span>                        | <span data-ttu-id="0ebff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ebff-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ebff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ebff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ebff-114">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0ebff-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="0ebff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ebff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ebff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ebff-116">Not supported.</span></span> |
| <span data-ttu-id="0ebff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ebff-117">Application</span></span>                            | <span data-ttu-id="0ebff-118">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0ebff-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ebff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ebff-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="0ebff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ebff-120">Request headers</span></span>

| <span data-ttu-id="0ebff-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0ebff-121">Name</span></span>          | <span data-ttu-id="0ebff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ebff-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0ebff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ebff-123">Authorization</span></span> | <span data-ttu-id="0ebff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ebff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ebff-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="0ebff-126">Content-type</span></span>  | <span data-ttu-id="0ebff-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ebff-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ebff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ebff-129">Request body</span></span>

<span data-ttu-id="0ebff-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ebff-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ebff-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0ebff-131">Parameter</span></span>    | <span data-ttu-id="0ebff-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ebff-132">Type</span></span>        | <span data-ttu-id="0ebff-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ebff-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ebff-134">Use</span><span class="sxs-lookup"><span data-stu-id="0ebff-134">use</span></span>|<span data-ttu-id="0ebff-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ebff-135">String</span></span>|<span data-ttu-id="0ebff-136">Semelhante à propriedade **use** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="0ebff-136">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="0ebff-137">f</span><span class="sxs-lookup"><span data-stu-id="0ebff-137">k</span></span>|<span data-ttu-id="0ebff-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ebff-138">String</span></span>|<span data-ttu-id="0ebff-139">Semelhante à propriedade **k** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="0ebff-139">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="0ebff-140">Este é o campo que é usado para enviar o segredo.</span><span class="sxs-lookup"><span data-stu-id="0ebff-140">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="0ebff-141">nbf</span><span class="sxs-lookup"><span data-stu-id="0ebff-141">nbf</span></span>|<span data-ttu-id="0ebff-142">Int64</span><span class="sxs-lookup"><span data-stu-id="0ebff-142">Int64</span></span>|<span data-ttu-id="0ebff-143">Semelhante à propriedade **NBF** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="0ebff-143">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="0ebff-144">exp</span><span class="sxs-lookup"><span data-stu-id="0ebff-144">exp</span></span>|<span data-ttu-id="0ebff-145">Int64</span><span class="sxs-lookup"><span data-stu-id="0ebff-145">Int64</span></span>|<span data-ttu-id="0ebff-146">Semelhante à propriedade **exp** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="0ebff-146">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="0ebff-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ebff-147">Response</span></span>

<span data-ttu-id="0ebff-148">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ebff-148">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ebff-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0ebff-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ebff-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ebff-150">Request</span></span>

<span data-ttu-id="0ebff-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ebff-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ebff-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ebff-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ebff-153">C#</span><span class="sxs-lookup"><span data-stu-id="0ebff-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ebff-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ebff-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ebff-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ebff-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ebff-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ebff-156">Response</span></span>

<span data-ttu-id="0ebff-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ebff-157">The following is an example of the response.</span></span>

> <span data-ttu-id="0ebff-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ebff-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


