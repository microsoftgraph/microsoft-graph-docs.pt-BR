---
title: 'trustFrameworkKeySet: uploadCertificate'
description: Carregue um certificado em um keyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 279794743f6f6b4cbd80fd9b3793195a73ff0e18
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433611"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="c3f3e-103">trustFrameworkKeySet: uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="c3f3e-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="c3f3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3f3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3f3e-105">Carregue um certificado em [um trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="c3f3e-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="c3f3e-106">A entrada é um valor codificado de base 64 do conteúdo do certificado.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="c3f3e-107">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="c3f3e-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f3e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3f3e-108">Permissions</span></span>

<span data-ttu-id="c3f3e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3f3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3f3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3f3e-111">Permission type</span></span>                        | <span data-ttu-id="c3f3e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3f3e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c3f3e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3f3e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3f3e-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f3e-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="c3f3e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3f3e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3f3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-116">Not supported.</span></span> |
| <span data-ttu-id="c3f3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3f3e-117">Application</span></span>                            | <span data-ttu-id="c3f3e-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f3e-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3f3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f3e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c3f3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f3e-120">Request headers</span></span>

| <span data-ttu-id="c3f3e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c3f3e-121">Name</span></span>          | <span data-ttu-id="c3f3e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f3e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c3f3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3f3e-123">Authorization</span></span> | <span data-ttu-id="c3f3e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c3f3e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c3f3e-126">Content-type</span></span> | <span data-ttu-id="c3f3e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3f3e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f3e-129">Request body</span></span>

<span data-ttu-id="c3f3e-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3f3e-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c3f3e-131">Parameter</span></span>    | <span data-ttu-id="c3f3e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3f3e-132">Type</span></span>        | <span data-ttu-id="c3f3e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3f3e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3f3e-134">key</span><span class="sxs-lookup"><span data-stu-id="c3f3e-134">key</span></span>|<span data-ttu-id="c3f3e-135">String</span><span class="sxs-lookup"><span data-stu-id="c3f3e-135">String</span></span>| <span data-ttu-id="c3f3e-136">Este é o campo para envio de conteúdo de certificado.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="c3f3e-137">O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="c3f3e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f3e-138">Response</span></span>

<span data-ttu-id="c3f3e-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3f3e-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3f3e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3f3e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3f3e-141">Request</span></span>

<span data-ttu-id="c3f3e-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3f3e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3f3e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadCertificate
Content-type: application/json

{
  "key": "key-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c3f3e-144">C#</span><span class="sxs-lookup"><span data-stu-id="c3f3e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3f3e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3f3e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3f3e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3f3e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3f3e-147">Java</span><span class="sxs-lookup"><span data-stu-id="c3f3e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3f3e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3f3e-148">Response</span></span>

<span data-ttu-id="c3f3e-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-149">The following is an example of the response.</span></span>

> <span data-ttu-id="c3f3e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3f3e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "kty": "oct",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


