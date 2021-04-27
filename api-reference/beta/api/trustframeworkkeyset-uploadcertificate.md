---
title: 'trustFrameworkKeySet: uploadCertificate'
description: Upload um certificado para um teclado.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 841a99797e737b79ee9d480b14a06c90a2bc2f48
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053416"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="8b1d7-103">trustFrameworkKeySet: uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="8b1d7-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="8b1d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b1d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b1d7-105">Upload um certificado para [um trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="8b1d7-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="8b1d7-106">A entrada é um valor codificado de base 64 do conteúdo do certificado.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="8b1d7-107">Este método retorna [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="8b1d7-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b1d7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b1d7-108">Permissions</span></span>

<span data-ttu-id="8b1d7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b1d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b1d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b1d7-111">Permission type</span></span>                        | <span data-ttu-id="8b1d7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b1d7-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b1d7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b1d7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b1d7-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b1d7-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="8b1d7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b1d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b1d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-116">Not supported.</span></span> |
| <span data-ttu-id="8b1d7-117">Application</span><span class="sxs-lookup"><span data-stu-id="8b1d7-117">Application</span></span>                            | <span data-ttu-id="8b1d7-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b1d7-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b1d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1d7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8b1d7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1d7-120">Request headers</span></span>

| <span data-ttu-id="8b1d7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8b1d7-121">Name</span></span>          | <span data-ttu-id="8b1d7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b1d7-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b1d7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b1d7-123">Authorization</span></span> | <span data-ttu-id="8b1d7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8b1d7-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="8b1d7-126">Content-type</span></span> | <span data-ttu-id="8b1d7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b1d7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1d7-129">Request body</span></span>

<span data-ttu-id="8b1d7-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b1d7-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8b1d7-131">Parameter</span></span>    | <span data-ttu-id="8b1d7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b1d7-132">Type</span></span>        | <span data-ttu-id="8b1d7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b1d7-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b1d7-134">key</span><span class="sxs-lookup"><span data-stu-id="8b1d7-134">key</span></span>|<span data-ttu-id="8b1d7-135">String</span><span class="sxs-lookup"><span data-stu-id="8b1d7-135">String</span></span>| <span data-ttu-id="8b1d7-136">Este é o campo para envio de conteúdo de certificado.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="8b1d7-137">O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="8b1d7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1d7-138">Response</span></span>

<span data-ttu-id="8b1d7-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b1d7-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b1d7-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b1d7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1d7-141">Request</span></span>

<span data-ttu-id="8b1d7-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b1d7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1d7-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b1d7-144">C#</span><span class="sxs-lookup"><span data-stu-id="8b1d7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b1d7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b1d7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b1d7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b1d7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b1d7-147">Java</span><span class="sxs-lookup"><span data-stu-id="8b1d7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b1d7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1d7-148">Response</span></span>

<span data-ttu-id="8b1d7-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-149">The following is an example of the response.</span></span>

> <span data-ttu-id="8b1d7-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b1d7-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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


