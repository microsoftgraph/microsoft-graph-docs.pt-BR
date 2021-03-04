---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: Carregue uma chave de formato PKCS 12 (PFX) em um keyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9de90df699c3086261321b38375373a00b464da1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433591"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="4f634-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="4f634-103">trustFrameworkKeySet: uploadPkcs12</span></span>

<span data-ttu-id="4f634-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f634-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f634-105">Carregue uma chave de formato PKCS12 (PFX) em [um trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="4f634-105">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="4f634-106">A entrada é um valor codificado de base 64 do conteúdo do certificado Pfx.</span><span class="sxs-lookup"><span data-stu-id="4f634-106">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="4f634-107">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="4f634-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f634-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f634-108">Permissions</span></span>

<span data-ttu-id="4f634-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f634-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f634-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f634-111">Permission type</span></span>                        | <span data-ttu-id="4f634-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f634-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f634-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f634-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f634-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f634-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="4f634-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f634-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f634-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f634-116">Not supported.</span></span> |
| <span data-ttu-id="4f634-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f634-117">Application</span></span>                            | <span data-ttu-id="4f634-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f634-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f634-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f634-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="4f634-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f634-120">Request headers</span></span>

| <span data-ttu-id="4f634-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4f634-121">Name</span></span>          | <span data-ttu-id="4f634-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f634-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4f634-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f634-123">Authorization</span></span> | <span data-ttu-id="4f634-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f634-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f634-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4f634-126">Content-type</span></span>  | <span data-ttu-id="4f634-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f634-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f634-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f634-129">Request body</span></span>

<span data-ttu-id="4f634-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f634-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f634-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4f634-131">Parameter</span></span>    | <span data-ttu-id="4f634-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f634-132">Type</span></span>        | <span data-ttu-id="4f634-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f634-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f634-134">key</span><span class="sxs-lookup"><span data-stu-id="4f634-134">key</span></span>|<span data-ttu-id="4f634-135">String</span><span class="sxs-lookup"><span data-stu-id="4f634-135">String</span></span>|<span data-ttu-id="4f634-136">Este é o campo para o envio de conteúdo pfx.</span><span class="sxs-lookup"><span data-stu-id="4f634-136">This is the field for sending pfx content.</span></span> <span data-ttu-id="4f634-137">O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado.</span><span class="sxs-lookup"><span data-stu-id="4f634-137">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="4f634-138">password</span><span class="sxs-lookup"><span data-stu-id="4f634-138">password</span></span>|<span data-ttu-id="4f634-139">String</span><span class="sxs-lookup"><span data-stu-id="4f634-139">String</span></span>|<span data-ttu-id="4f634-140">Este é o campo para enviar a senha para o conteúdo PFX.</span><span class="sxs-lookup"><span data-stu-id="4f634-140">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="4f634-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f634-141">Response</span></span>

<span data-ttu-id="4f634-142">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f634-142">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f634-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4f634-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f634-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f634-144">Request</span></span>

<span data-ttu-id="4f634-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f634-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f634-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f634-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4f634-147">C#</span><span class="sxs-lookup"><span data-stu-id="4f634-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f634-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f634-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f634-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f634-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f634-150">Java</span><span class="sxs-lookup"><span data-stu-id="4f634-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadpkcs12-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f634-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f634-151">Response</span></span>

<span data-ttu-id="4f634-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f634-152">The following is an example of the response.</span></span>

> <span data-ttu-id="4f634-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f634-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "use": "sig",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


